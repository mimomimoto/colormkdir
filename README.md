<div align="center">
  <img width="300" alt="colormkdir logo" src="https://user-images.githubusercontent.com/99246880/224245097-6d4617a3-6987-43ad-81af-6b4696e7c9fc.png" />
</div>

**Table of Contents**
- [colormkdir](#colormkdir)
- [Demo](#demo)
- [Installation](#Installation)
    - [Use Homebrew](#use_homebrew)
    - [Manual Installation](#manual_installation)
- [Usage](#usage)
    - [Create color list](#Create_color_list)
    - [Update color list](#Update_color_list)
    - [Make directory in specified color](#Make_directory_in_specified_color)
    - [Change directory color as specified color](#Change_directory_color_as_specified_color)
    - [Help command](#Help_command)

# colormkdir
`colormkdir` is a CLI for macOS to customize folder color. 
It can make directory in specified color. Also, it can manage color list by editing json file.

# Demo
![demo.gif](https://user-images.githubusercontent.com/99246880/224244901-8ff520df-f383-4c35-a185-dba17773eabd.gif)

# Installation
**Supported platforms**

* **macOS**

## Use Homebrew

```
brew install mimomimoto/tap/colormkdir
```
`colormkdir` use python3 and you should install some libraries.

```
pip install pyobjc pillow glob2
```
## Manual Installation
1. git clone this repository.
2. Write PATH to `~/.zshrc`.
3. Change `colormkdir` permission by using chmod.
4. run `source ~/.zshrc`.
5. `pip install pyobjc pillow glob2 `

> `colormkdir` use your global python environment. If you don't want to install these libraries in your global environment, you should edit colormkdir.sh (line 64).

# Usage
## Create color list
Color list is managed by JSON file. (In my case, the file path is '/opt/homebrew/Cellar/colormkdir/0.0.1/libexec/color_list.json') You need to decide `color name` and `color code` as shown below. (It is default definition)
```
{
    "r":"#ff0000",
    "b":"#1e90ff",
    "g":"#3cb371",
    "y":"#ffff00",
    "p":"#9400d3",
    "o":"#ff7f50"
}
```

## Update color list
After change color list, you need to run command for updating color list. 
```
colormkdir -u
```

## Make directory in specified color
```
colormkdir -m [value] <directory name>
```
[value] is `color name` defined in color list. If directory name is already exsisted, it will be error.

## Change directory color as specified color
```
colormkdir -c [value] <directory name>
```
[value] is `color name` defined in color list. If directory name is not exsisted, it will be error.

## Help command
```
colormkdir -h
```


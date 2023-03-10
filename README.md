<div align="center">
  <img width="300" alt="colormkdir logo" src="https://user-images.githubusercontent.com/99246880/224245097-6d4617a3-6987-43ad-81af-6b4696e7c9fc.png" />
</div>

**Table of Contents**
- [colormkdir](#colormkdir)
- [Demo](#demo)
- [Installation](#Installation)
- [Usage](#usage)

# colormkdir
`colormkdir` is a CLI for macOS to customize folder color. 
It can make directory in specified color. Also, it can manage color list by editing json file.

# Demo
![demo.gif](https://user-images.githubusercontent.com/99246880/224244901-8ff520df-f383-4c35-a185-dba17773eabd.gif)

# Installation
Use [Homebrew](https://brew.sh/).

```
brew install mimomimoto/tap/colormkdir
```
`colormkdir` use python3 and you should install some libraries.

```
pip install pyobjc
pip install pillow
pip install glob2
```

> `colormkdir` use your global python environment. If you don't want to install these libraries in your global environment, you should edit colormkdir.sh (line 64).

# Usage
## Create color list


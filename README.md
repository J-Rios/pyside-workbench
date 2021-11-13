# vscode-skelly-pyside

A simple pyside6 (QT-6) development base project skelleton for vscode.

## Documentation

Python QT Documentation:  
[https://doc.qt.io/qtforpython/](https://doc.qt.io/qtforpython/)

QT Documentation:  
[https://doc.qt.io/](https://doc.qt.io/)


## Requeriments

For PySide6, you need to use [Python 3](https://www.python.org/downloads/) (minimum version: Python 3.6), and also install pyside6 using pip.

For Linux users in a Debian based system:

```bash
sudo apt-get update
sudo apt-get install libopengl0 libegl1
sudo apt-get install freeglut3 freeglut3-dev
sudo apt-get install python3
sudo apt-get install python3-pip
python3 -m pip install PySide6==6.2.1
```

Of course, you need to install [vscode](https://code.visualstudio.com/download), and the following extensions on it:

```text
Python
Qt for Python
```

Also, you can install the next recommended extensions:

```text
QML
Color Manager
```

## Notes

- If you want to use it in Windows with WSL-1, maybe you should need to install an X Graphical Server for Windows like [XMing](https://sourceforge.net/projects/xming/) and setup a DISPLAY enviroment variable:

```bash
export DISPLAY=:0
grep -qxF "export DISPLAY=:0" ~/.bashrc || printf "\n#Setup Display\nexport DISPLAY=:0\n\n" >> ~/.bashrc
```

- Remember that XMing must be running to launch PySide applications from WSL-1.

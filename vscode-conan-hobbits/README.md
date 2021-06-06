
# Developing Hobbits with Visual Studio Code, Conan, and Qt Creator

Visual Studio Code (VSCode) is a very popular and flexible text editor. This
guide and accompanying config files should help you get set up developing
hobbits with VSCode as your primary editor.

In the setup described here, Conan will be used to resolve dependencies, and Qt
Creator will be used to edit Qt *.ui form files.


## Prerequisites

You should have the following tools installed:

 - A modern C++ toolchain
 - CMake 3.12+
 - Python 3.5+
 - Conan (latest version installed via pip)
 - Qt Creator
 - VSCode and its official Microsoft C++ and Python extensions


## Setting up

After cloning hobbits, place the `.vscode` folder included here directly into
the root directory. It should enable you to execute the "Conan initialize" task
in VSCode (Ctrl-Shift-P -> Tasks: Run Task -> Conan initialize.) Once this is
done, you can use the built-in debugging tab in VSCode to launch and debug the
hobbits gui.

Editing the XML-formatted *.ui Qt form files manually is not recommended, so
there is a "dummy" Qt project file in the hobbits repo at
`src/hobbits-qt-ui-forms.pro` that you can open in Qt Creator to edit your ui
files.
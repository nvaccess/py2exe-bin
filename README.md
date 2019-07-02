# py2exe-bin
NVDA's py2exe dependency

This repository fulfils NVDA's build dependency on py2exe from https://github.com/albertosottile/py2exe.
Currently, py2exe 0.9.3.2 (in development, commit b372a8e from https://github.com/albertosottile/py2exe/pull/13) is used.
It was created with the following command: `pip3 install -t ./ <path_to_local_git_clone_of_py2exe>`

Py2exe relies on pywin32, which is also included in this repository.
The pywin32 distribution was created using the following steps:

1. Create a new directory.

1. In the new dirctory, execute the following command: `pip3 install -t ./ pywin32`

1. Copy the following dirctories and files from the populated directory to the root of this repository:

	* All files from the root of the `win32` dirctory
	* All files from the `win32/lib` dirctory
	* All files from the `pywin32_system32` dirctory
	* The complete `win32com` dirctory
	* The complete `win32comext` directory
	* The `pythoncom.py` module
	
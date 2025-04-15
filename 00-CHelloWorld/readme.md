# SSL  
A. MinGW-w64  
B. GCC 14.2.0  
C. C23

### Obtención de la información del compilador.
-  El compilador y la versión lo averigüe a través de escribir en la terminal el comando        ¨gcc --version¨
-  La versión de C que compila el compilador fue a través de la edición del archivo tasks.json, le ingrese el siguiente código:
  ~~~
  {
	"version": "2.0.0",
	"tasks": [
		{
			"type": "cppbuild",
			"label": "C/C++: gcc.exe build active file",
			"command": "C:\\Users\\marco\\Documents\\winlibs-x86_64-posix-seh-gcc-14.2.0-llvm-19.1.7-mingw-w64ucrt-12.0.0-r3\\mingw64\\bin\\gcc.exe",
			"args": [
				"-fdiagnostics-color=always",
				"-std=c23",
				"-g",
				"${file}",
				"-o",
				"${fileDirname}\\${fileBasenameNoExtension}.exe"
			],
			"options": {
				"cwd": "${fileDirname}"
			},
			"problemMatcher": [
				"$gcc"
			],
			"group": "build",
			"detail": "compiler: C:\\Users\\marco\\Documents\\winlibs-x86_64-posix-seh-gcc-14.2.0-llvm-19.1.7-mingw-w64ucrt-12.0.0-r3\\mingw64\\bin\\gcc.exe"
		},
		{
			"type": "cppbuild",
			"label": "C/C++: clang.exe build active file",
			"command": "C:\\Users\\marco\\Documents\\winlibs-x86_64-posix-seh-gcc-14.2.0-llvm-19.1.7-mingw-w64ucrt-12.0.0-r3\\mingw64\\bin\\clang.exe",
			"args": [
				"-fcolor-diagnostics",
				"-fansi-escape-codes",
				"-std=c23",
				"-g",
				"${file}",
				"-o",
				"${fileDirname}\\${fileBasenameNoExtension}.exe"
			],
			"options": {
				"cwd": "${fileDirname}"
			},
			"problemMatcher": [
				"$gcc"
			],
			"group": "build",
			"detail": "compiler: C:\\Users\\marco\\Documents\\winlibs-x86_64-posix-seh-gcc-14.2.0-llvm-19.1.7-mingw-w64ucrt-12.0.0-r3\\mingw64\\bin\\clang.exe"
		}
	]
}

  ~~~ 

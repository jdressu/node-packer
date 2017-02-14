# Node.js Compiler

Compiling your Node.js application into a single executable.

http://enclose.io

[![Travis CI status](https://travis-ci.org/pmq20/node-compiler.svg?branch=master)](https://travis-ci.org/pmq20/node-compiler)
[![AppVeyor status](https://ci.appveyor.com/api/projects/status/gap9xne0rayjtynp/branch/master?svg=true)](https://ci.appveyor.com/project/pmq20/node-compiler/branch/master)

## Nightly Builds: Feb 10, 2017

### Virginia, United States mirror

| Operating System | Architecture | Download Link                                 |
|:----------------:|:------------:|-----------------------------------------------|
|      Windows     |      x86     | http://enclose.io/2017feb10/nodec.exe         |
|       macOS      |     x86-64   | http://enclose.io/2017feb10/nodec-darwin-x64  |
|       Linux      |     x86-64   | http://enclose.io/2017feb10/nodec-linux-x64   |

### 中国北京镜像

|      操作系统     |      架构     | 下载链接                                                                    |
|:----------------:|:------------:|---------------------------------------------------------------------------|
|      Windows     |      x86     | http://enclose-io.oss-cn-beijing.aliyuncs.com/2017feb10/nodec.exe         |
|       macOS      |     x86-64   | http://enclose-io.oss-cn-beijing.aliyuncs.com/2017feb10/nodec-darwin-x64  |
|       Linux      |     x86-64   | http://enclose-io.oss-cn-beijing.aliyuncs.com/2017feb10/nodec-linux-x64   |


## Install

On Windows, you could just download `nodec.exe` and run it from the Visual Studio Command Prompt.

On macOS, you could download and install into your system directory like this:

    sudo curl http://enclose.io/2017feb10/nodec-darwin-x64 > /usr/local/bin/nodec
    chmod +x /usr/local/bin/nodec
    nodec

On Linux, you could download and install into your system directory like this:

    sudo curl http://enclose.io/2017feb10/nodec-linux-x64 > /usr/local/bin/nodec
    chmod +x /usr/local/bin/nodec
    nodec

## Usage

    nodec [...OPTIONS..] ENTRANCE
      -r, --root=DIR                   Speicifies the path to the root of the application
      -o, --output=FILE                Speicifies the path of the output file
      -d, --tmpdir=DIR                 Speicifies the directory for temporary files
          --make-args=ARGS             Passes extra arguments to make
          --vcbuild-args=ARGS          Passes extra arguments to vcbuild.bat
          --npm=FILE                   Speifices the path of npm
          --debug                      Enable debug mode
      -v, --version                    Prints the version of nodec and exit
          --node-version               Prints the version of the Node.js runtime and exit
      -h, --help                       Prints this help and exit

## Example

    git clone --depth 1 https://github.com/jashkenas/coffeescript.git
    cd coffeescript
    nodec bin/coffee
    ./a.out (or a.exe on Windows)

## See Also

- [Libsquash](https://github.com/pmq20/libsquash): portable, user-land SquashFS implementation that can be easily linked and embedded within your application.

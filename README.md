# Installation

1. cmake: https://cmake.org/download/
2. .NET: https://dotnet.microsoft.com/en-us/download

If on Windows:

3. Visual Studio Community: https://visualstudio.microsoft.com/vs/community/

# Build

Run the following commands from the project root:

## C#

```commandline
cd csharp
dotnet build
```

## C++

If on Linux or MacOS:

```commandline
cd cpp/lib/cryptopp
make
```

```commandline
cd cpp
mkdir build && cd build
cmake .
make
```

If on Windows:

Open the project in Visual Studio. If it complains about an outdated toolset, change to the newer toolset in properties. Build project lib and build project DLL. Copy DLL to the folder where `cpp.exe` is located, most likely `cpp\build\Debug`.

```commandline
cd cpp\build
cmake --build .
```

# Run

## C#

Run the following commands in the `csharp` directory.

Encrypt a message:

```commandline
dotnet build 1
```

Decrypt a message:

```commandline
dotnet build 2
```

## C++

Run the following commands in the `cpp\build\Debug` directory (or wherever the executable resides).

Encrypt a message:

```commandline
.\cpp.exe 1
```

Decrypt a message:

```commandline
.\cpp.exe 2
```

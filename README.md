# Runtime.Events.Azure

This contains an Azure CosmosDB implementation for EventStore.  
The implementation will create the required collections / server side artifacts but expects the CosmosDB to be created.
To run the specs, you are required to provide three environmental variables:

"EVENTSTORE_AZURE_URL" - the url to the CosmosDB
"EVENTSTORE_AZURE_DATABASE" - the name of the CosmosDB instance
"EVENTSTORE_AZURE_AUTHKEY" - the authkey for authentication

## Cloning

This repository has sub modules, clone it with:

```shell
$ git clone --recursive <repository url>
```

If you've already cloned it, you can get the submodules by doing the following:

```shell
$ git submodule update --init --recursive
```

## Building

All the build things are from a submodule.
To build, run one of the following:

Windows:

```shell
$ Build\build.cmd
```

Linux / macOS

```shell
$ Build\build.sh
```

## Packages

| Platform | Production   | From CI  |
| ------- | ------- | ------ |
| Runtime.Events.Azure | [![NuGet](https://img.shields.io/nuget/v/dolittle.svg)](https://www.nuget.org/packages?q=dolittle) | [![MyGet](https://img.shields.io/myget/dolittle/vpre/dolittle.svg)](https://www.myget.org/gallery/dolittle) |

## Build Status

| Project | AppVeyor | 
| -------- | ------ |
| Runtime.Events.Azure | [![Build status](https://ci.appveyor.com/api/projects/status/9ti5wbo8mermf6iw?svg=true)](https://ci.appveyor.com/project/Dolittle/runtime-events-azure) |

## Visual Studio

You can open the `.sln` file in the root of the repository and just build directly.

## VSCode

From the `Build` submdoule there is also a .vscode folder that gets a symbolic link for the root. This means you can open the
root of the repository directly in Visual Studio Code and start building. There are quite a few build tasks, so click F1 and type "Run Tasks" and select the "Tasks: Run Tasks"
option and then select the build task you want to run. It is folder sensitive and will look for the nearest `.csproj` file based on the file you have open.
If it doesn't find it, it will pick the `.sln` file instead.

## More details

To learn more about the projects of Dolittle and how to contribute, please go [here](https://github.com/dolittle/Home).

## Getting Started

Go to our [documentation site](http://www.dolittle.io) and learn more about the project and how to get started.
Samples can also be found [here](https://github.com/Dolittle-Samples).
You can find entropy projects [here](https://github.com/Dolittle-Entropy).

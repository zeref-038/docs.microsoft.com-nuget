---
title: dotnet CLI NuGet commands
description: A short reference for NuGet-related commands using the dotnet command-line interface.
author: karann-msft
ms.author: karann
ms.date: 06/24/2019
ms.topic: conceptual
---

# dotnet CLI commands

The `dotnet` command-line interface (CLI), which runs on Windows, Mac OS X, and Linux, provides a number of essential commands such as installing, restoring, and publishing packages. If dotnet satisfies your needs, it's not necessary to use `nuget.exe`.

For examples of using these commands to consume packages, see [Install and manage packages using the dotnet CLI](../consume-packages/install-use-packages-dotnet-cli.md). For examples of using these commands to create packages, see [Create and publish a package using the dotnet CLI](../quickstart/create-and-publish-a-package-using-the-dotnet-cli.md).

For the complete command reference on `dotnet` CLI, see [.NET Core command-line interface (CLI) tools](/dotnet/core/tools/?tabs=netcore2x).

## Package consumption

- [**dotnet add package**](/dotnet/core/tools/dotnet-add-package): Adds a package reference to the project file, then runs `dotnet restore` to install the package.
- [**dotnet remove package**](/dotnet/core/tools/dotnet-remove-package): Removes a package reference from the project file.
- [**dotnet restore**](/dotnet/core/tools/dotnet-restore?tabs=netcore2x): Restores the dependencies and tools of a project. As of NuGet 4.0, this runs the same code as `nuget restore`.
- [**dotnet nuget locals**](/dotnet/core/tools/dotnet-nuget-locals): Lists locations of the *global-packages*, *http-cache*, and *temp* folders and clears the contents of those folders.

## NuGet configuration
- [**dotnet new nugetconfig**](/dotnet/core/tools/dotnet-new): Creates a [`nuget.config`](../reference/nuget-config-file.md) file to configure NuGet's behavior.
- [**dotnet nuget list source**](/dotnet/core/tools/dotnet-nuget-list-source): Lists sources located in the user scope configuration file or a specified configuration file.
- [**dotnet nuget add source**](/dotnet/core/tools/dotnet-nuget-add-source): Adds a new source in the user scope configuration file or a specified configuration file.
- [**dotnet nuget update source**](/dotnet/core/tools/dotnet-nuget-update-source): Updates a named source in the user scope configuration file or a specified configuration file.
- [**dotnet nuget remove source**](/dotnet/core/tools/dotnet-nuget-remove-source): Removes a named source in the user scope configuration file or a specified configuration file.
- [**dotnet nuget disable source**](/dotnet/core/tools/dotnet-nuget-disable-source): Disables a named source in the user scope configuration file or a specified configuration file.
- [**dotnet nuget enable source**](/dotnet/core/tools/dotnet-nuget-enable-source): Enables a named source in the user scope configuration file or a specified configuration file.


## Package creation

- [**dotnet pack**](/dotnet/core/tools/dotnet-pack?tabs=netcore2x): Packs the code into a NuGet package.
- [**dotnet nuget push**](/dotnet/core/tools/dotnet-nuget-push): Publishes a package to a NuGet server. Applicable to nuget.org, Azure Artifacts, and [third-party NuGet servers](../hosting-packages/overview.md).
- [**dotnet nuget delete**](/dotnet/core/tools/dotnet-nuget-delete): Deletes or unlists a package from a NuGet server. Applicable to nuget.org, Azure Artifacts, and [third-party NuGet servers](../hosting-packages/overview.md).

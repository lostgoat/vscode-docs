---
Order: 4
Area: remote
TOCTitle: Visual Studio Online
PageTitle: Developing with Visual Studio Online
ContentId: 8d30ed21-208f-4b4e-8510-5a4a33c42618
MetaDescription: Using Visual Studio Code Online
DateApproved: 10/9/2019
---
# Visual Studio Online

[Visual Studio Online](https://docs.microsoft.com/visualstudio/online/overview/what-is-vsonline) provides cloud-powered development environments for any activity - whether it's a long-term project, or a short-term task like reviewing a pull request. You can work with these environments from three possible clients: Visual Studio Code, a browser-based version of VS Code, or the Visual Studio IDE (currently in Private Preview).

## Environments

An [environment](https://docs.microsoft.com/visualstudio/online/overview/what-is-vsonline#environments) is the "backend" half of Visual Studio Online. It's where all of the compute associated with software development happens: compiling, debugging, restoring, etc. When you need to work on a new project, pick up a new task, or review a PR, you can simply spin up a Cloud-hosted environment, and Visual Studio Online takes care of configuring it correctly. It automatically configures everything you need to work on your project: the source code, runtime, compiler, debugger, editor, custom dotfile configurations, relevant editor extensions and more.

## Customization

Visual Studio Online's environments are fully customizable on a per project basis. This is accomplished by including a [devcontainer.json](/docs/remote/containers.md#creating-a-devcontainerjson-file) file in the project's repository.

Example customizations include:

* Setting which Linux-based operating system to use
* Automatically installing various tools, runtimes, and frameworks
* Forwarding commonly used ports
* Setting environment variables
* Configuring editor settings and installing preferred extensions

See [VS Online Configuring documentation](https://docs.microsoft.com/visualstudio/online/reference/configuring) for VS Online specific `devcontainer.json` settings.

## Dotfile per user configuration

Dotfiles are files whose filename begins with a dot (.). They typically contain configuration information for various applications and can control how terminals, editors, source control, and various other tools behave. `.bashrc`, `.gitignore` and `.editorconfig` are examples of dotfiles commonly used by developers.

You can specify a GitHub repo containing your dotfiles, a target location for the files, as well as install commands when creating a VS Online environment.

See the [VS Online Personalizing documentation](https://docs.microsoft.com/visualstudio/online/reference/personalizing) to learn how to add your dotfile configurations to an environment.

## Getting started

The Visual Studio Online documentation has Quickstarts for all three clients. They will fast track you through signing in to VS Online, creating your first environment, and connecting to it with your preferred client:

* [VS Online in VS Code](https://docs.microsoft.com/visualstudio/online/quickstarts/vscode) - Use VS Code to connect and work in your VS Online environment.
* [VS Online in the browser](https://docs.microsoft.com/visualstudio/online/quickstarts/browser) - Connect to your VS Online environment through a browser-based editor.
* [VS Online in Visual Studio IDE](https://docs.microsoft.com/visualstudio/online/quickstarts/vs) - Try out the Visual Studio IDE Private Preview with VS Online.

## How-to guides

In addition to the Quickstarts, there are How-to guides, which go into more detail about managing and configuring your environments:

* [How-to guide: Visual Studio Code](https://docs.microsoft.com/visualstudio/online/how-to/vscode) - Create and configure an environment from the VS Code client.
* [How-to guide: Browser](https://docs.microsoft.com/visualstudio/online/how-to/browser) - Create and configure a VS Online environment with only a browser.

## Self-hosted environments

You can even connect your own self-hosted environments to Visual Studio Online at no cost.

## Questions or feedback

If you have questions, you can consult the VS Online [Troubleshooting guide](https://docs.microsoft.com/visualstudio/online/resources/troubleshooting) and [FAQ](https://docs.microsoft.com/visualstudio/online/resources/faq). You can provide [Feedback](https://docs.microsoft.com/visualstudio/online/resources/feedback) through the [vsoline](https://github.com/MicrosoftDocs/vsonline) GitHub repository.
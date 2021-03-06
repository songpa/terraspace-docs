---
title: Lookups
---

The [Project Structure]({% link _docs/intro/structure.md %}) docs explains how modules and stacks are generally defined in the `app` folder. Modules and stacks can also be defined in the `vendor` folder also. The vendor folder neatly organizes 3rd party vendor modules. Terraspace commands like `terraspace build` and `terraspace run` look for modules to build from both app and vendor folders.

## Example

Here's an example with some modules in the vendor folder.

    ├── app
    │   └── modules
    │       └── instance
    └── vendor
        └── modules
            ├── database
            └── network

In this case, there are database and network 3rd parties modules. There's also a normal project module called instance.

Note: When there are 2 modules with the same name in both the app and vendor folder, the app folder wins.

## terraspace bundle

The vendor additional lookup location can be particularly useful with modules declared in a [Terrafile]({% link _docs/terrafile.md %}). You can add modules to your Terrafile definition and download them to the `vendor/modules` folder with:

    terraspace bundle

<p align="center">
    <a href="https://appwrite.io" target="_blank"><img width="260" height="39" src="https://appwrite.io/images/github-logo.png" alt="Appwrite Logo"></a>
    <br />
    <br />
    <b>A complete backend solution for your [Flutter / Vue / Angular / React / NodeJS / iOS / Android / *ANY OTHER*] app</b>
    <br />
    <br />
</p>

[![Hacktoberfest](https://badgen.net/badge/hacktoberfest/friendly/pink)](CONTRIBUTING.md)
[![Discord](https://img.shields.io/discord/564160730845151244?label=discord)](https://discord.gg/GSeTUeA)
[![Docker Pulls](https://badgen.net/docker/pulls/appwrite/appwrite)](https://travis-ci.org/appwrite/appwrite)
[![Travis CI](https://badgen.net/travis/appwrite/appwrite?label=build)](https://travis-ci.org/appwrite/appwrite)
[![Twitter Account](https://badgen.net/twitter/follow/appwrite_io?label=twitter)](https://twitter.com/appwrite_io)
[![Follow Appwrite on StackShare](https://badgen.net/badge/follow%20on/stackshare/blue)](https://stackshare.io/appwrite)

Appwrite is an end-to-end backend server for Web, Mobile, Native, or Backend apps packaged as a set of Docker microservices. Appwrite abstract the complexity and repetitiveness required to build a modern backend API from scratch to allow you to build secure apps faster.

Using Appwrite, you can easily integrate your app with user authentication & multiple sign-in methods, a database for storing and querying users and team data, storage and file management, image manipulation, schedule CRON tasks, and [more services](https://appwrite.io/docs).

[https://appwrite.io](https://appwrite.io)

![Appwrite](public/images/github.png)

Table of Contents:

- [Installation](#installation)
  - [Unix](#unix)
  - [Windows](#windows)
    - [CMD](#cmd)
    - [PowerShell](#powershell)
- [Getting Started](#getting-started)
  - [Services](#services)
  - [SDKs](#sdks)
    - [Client](#client)
    - [Server](#server)
- [Security](#security)
- [Follow Us](#follow-us)
- [Contributing](#contributing)
- [License](#license)
      
## Installation

Appwrite backend server is designed to run in a container environment. Running your server is as easy as running one command from your terminal. You can either run Appwrite on your localhost using docker-compose or on any other container orchestration tool like Kubernetes, Docker Swarm or Rancher.

The easiest way to start running your Appwrite server is by running our docker-compose file. Before running the installation command make sure you have [Docker](https://www.docker.com/products/docker-desktop) installed on your machine:

### Unix

```bash
docker run -it --rm \
    --volume /var/run/docker.sock:/var/run/docker.sock \
    --volume "$(pwd)"/appwrite:/install/appwrite:rw \
    -e version=0.6.2 \
    appwrite/install
```

### Windows

#### CMD

```cmd
docker run -it --rm ^
    --volume //var/run/docker.sock:/var/run/docker.sock ^
    --volume "%cd%"/appwrite:/install/appwrite:rw ^
    -e version=0.6.2 ^
    appwrite/install
```

#### PowerShell

```powershell
docker run -it --rm ,
    --volume /var/run/docker.sock:/var/run/docker.sock ,
    --volume ${pwd}/appwrite:/install/appwrite:rw ,
    -e version=0.6.2 ,
    appwrite/install
```

Once the Docker installation completes, go to http://localhost to access the Appwrite console from your browser. Please note that on non-linux native hosts, the server might take a few minutes to start after installation completes.


For advanced production and custom installation, check out our Docker [environment variables](docs/tutorials/environment-variables.md) docs. You can also use our public [docker-compose.yml](https://appwrite.io/docker-compose.yml) file to manually set up and environment.

## Getting Started

Getting started with Appwrite is as easy as creating a new project, choosing your platform and integrating its SDK in your code. You can easily get started with your platform of choice by reading one of our Getting Started tutorials.

* [Getting Started for Web](https://appwrite.io/docs/getting-started-for-web)
* [Getting Started for Flutter](https://appwrite.io/docs/getting-started-for-flutter)
* [Getting Started for Server](https://appwrite.io/docs/getting-started-for-server)
* Getting Started for Android (soon...)
* Getting Started for iOS (soon...)

### Services

* [**Account**](https://appwrite.io/docs/client/account) - Manage current user authentication and account. Track and manage the user sessions, devices, sign-in methods, and security logs.
* [**Users**](https://appwrite.io/docs/server/users) - Manage and list all project users when in admin mode.
* [**Teams**](https://appwrite.io/docs/client/teams) - Manage and group users in teams. Manage memberships, invites, and user roles within a team.
* [**Database**](https://appwrite.io/docs/client/database) - Manage database collections and documents. Read, create, update, and delete documents and filter lists of documents collections using an advanced filter with graph-like capabilities.
* [**Storage**](https://appwrite.io/docs/client/storage) - Manage storage files. Read, create, delete, and preview files. Manipulate the preview of your files to fit your app perfectly. All files are scanned by ClamAV and stored in a secure and encrypted way.
* [**Locale**](https://appwrite.io/docs/client/locale) - Track your user's location, and manage your app locale-based data.
* [**Avatars**](https://appwrite.io/docs/client/avatars) - Manage your users' avatars, countries' flags, browser icons, credit card symbols, and generate QR codes.

For the complete API documentation, visit [https://appwrite.io/docs](https://appwrite.io/docs). For more tutorials, news and announcements check out our [blog](https://medium.com/appwrite-io) and [Discord Server](https://discord.gg/GSeTUeA).

### SDKs

Below is a list of currently supported platforms and languages. If you wish to help us add support to your platform of choice, you can go over to our [SDK Generator](https://github.com/appwrite/sdk-generator) project and view our [contribution guide](https://github.com/appwrite/sdk-generator/blob/master/CONTRIBUTING.md).

#### Client
* ✅ [Web](https://github.com/appwrite/sdk-for-js) (Maintained by the Appwrite Team)
* ✅ [Flutter](https://github.com/appwrite/sdk-for-flutter) (Maintained by the Appwrite Team)

#### Server
* ✅ [NodeJS](https://github.com/appwrite/sdk-for-node) (Maintained by the Appwrite Team)
* ✅ [PHP](https://github.com/appwrite/sdk-for-php) (Maintained by the Appwrite Team)
* ✅ [Deno](https://github.com/appwrite/sdk-for-deno) - **Beta** (Maintained by the Appwrite Team)
* ✅ [Ruby](https://github.com/appwrite/sdk-for-ruby) - **Beta** (Maintained by the Appwrite Team)
* ✅ [Python](https://github.com/appwrite/sdk-for-python) - **Beta** (Maintained by the Appwrite Team)
* ✅ [Go](https://github.com/appwrite/sdk-for-go) **Work in progress** (Maintained by the Appwrite Team)
* ✅ [Dart](https://github.com/appwrite/sdk-for-dart) **Work in progress** (Maintained by the Appwrite Team)

Looking for more SDKs? - Help us by contributing a pull request to our [SDK Generator](https://github.com/appwrite/sdk-generator)!

## Contributing

All code contributions - including those of people having commit access - must go through a pull request and approved by a core developer before being merged. This is to ensure proper review of all the code.

We truly ❤️ pull requests! If you wish to help, you can learn more about how you can contribute to this project in the [contribution guide](CONTRIBUTING.md).

## Security

For security issues, kindly email us [security@appwrite.io](mailto:security@appwrite.io) instead of posting a public issue in GitHub.

## Follow Us

Join our growing community around the world! Follow us on [Twitter](https://twitter.com/appwrite_io), [Facebook Page](https://www.facebook.com/appwrite.io), [Facebook Group](https://www.facebook.com/groups/appwrite.developers/) or join our live [Discord server](https://discord.gg/GSeTUeA) for more help, ideas, and discussions.

## License

This repository is available under the [BSD 3-Clause License](./LICENSE).

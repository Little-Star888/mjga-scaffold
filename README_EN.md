# Make Java Great Again!

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
![logo.png](asset/logo.png)

🏆🎖️🥇🥈🥉🏅

- [English](README_EN.md)
- [中文](README_CN.md)

## Why is Mjga Unique?

[Mjga](https://www.mjga.cc) is a newly designed, cloud-native-based modern Java Web scaffolding framework. It features:

- Containerized applications
- Plug-and-play components
- Widely acclaimed unit testing
- Custom metadata

### 🥝 Template Selection

![option_cn.png](asset/option_en.png)

### 🍅 Component Configuration

![stack_cn.png](asset/stack_en.png)

### 🍹 Custom Metadata

![meta_cn.png](asset/meta_en.png)

#### Containerization and Cloud-Native

1. Manage the entire lifecycle and configuration of the application via `docker-compose.yml`.
2. Customize all configurations through the `.env` file.
3. Deliver the entire application and its ecosystem components via `docker-compose.yml`.

#### Out-of-the-Box

1. Integrates common basic business functionalities such as authentication, permission management, and cache abstraction.
2. Code Check & Format, CI/CD Plugin, Docker Integration are all ready to use out of the box.
3. Comprehensive, design-driven, and environment-isolated unit testing.

#### Modernization

1. Modern: Technology choices align with the latest trends in the open-source community.
2. Configurable: Supports component selection on the web.
3. Best Practices: Every variable, function, module, and component is designed with best practices in mind.
4. Focused Boundaries: Stays within its functional boundaries, avoiding an "All In One" approach.

### Quick Start

**Confirm Environment Variables and Execution Permissions**

```shell
# confirm .env and make sure process can use it
vim ${projectRoot}/.env
# confirm gradlew executable (unix-like OS)
chmod 755 ${projectRoot}/gradlew
```

**[Install Docker and Start Containers](https://docs.docker.com/engine/install/)**

```shell
cd ${projectRoot}
docker compose up -d database
docker compose build web
docker compose up -d web
```

**(Optional) Start Locally**

```shell
# confirm .env and gradle.properties make sure process can use it
vim ${projectRoot}/.env
docker compose up -d database
./gradlew jooqCodegen
${projectRoot}/gradlew bootRun
```

### Common Tools

**Compile the Project and Generate Table Mapping Objects and Data Access Layer Based on Database Schema**

```shell
# generate schema mapping codes
./gradlew jooqCodegen
# output ->
# projectRootDir/build/generated-sources
# └── org.jooq.generated
#    └── tables # table mapping
#       ├── daos # Data Access Layer
#       ├── pojos # mapping dto
#       └── records # jooq query record
```

**Global Code Formatting**

```shell
./gradlew spotlessApply
```

**Global Code Inspection**

```shell
./gradlew pmdMain
```

**Unit Testing**

```shell
# will automatically generate jacocoTestReport
./gradlew test
```

[更多文档请点击...](https://www.mjga.cc/doc/db-first)


## 🍓 Test Report

![cover](https://www.mjga.cc/report/cover.png)

![summary](https://www.mjga.cc/report/summary.png)

## 🍟 Miscellaneous

1. This repository is primarily for code display and issue collection. The code may lag behind the version available for
   download from the product's official website.
2. Please submit any feedback, discussions, or bugs to the issue tracker, and I will handle them seriously.
3. I also welcome any ideas from other communities and will actively participate in the replies.
4. More new video tutorials are being recorded, please stay tuned.
5. Promote Mjga to your colleagues and friends, and let Java be great again.

## 🔮 User Community

[![Static Badge](https://img.shields.io/badge/blog-black?style=flat&logo=dev.to&logoSize=auto)](https://dev.to/ccmjga)
[![Static Badge](https://img.shields.io/badge/homepage-white?style=flat&logo=homepage&logoColor=%23FF0074)](https://www.mjga.cc)
[![Static Badge](https://img.shields.io/badge/twitter-blue?style=flat&logo=x)](https://x.com/Mjga212318)
[![Static Badge](https://img.shields.io/badge/discord-white?style=flat&logo=discord)](https://discord.com/invite/3XhyjEPn)

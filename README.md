# onecx-quarkus3-parent

Maven parent for all Quarkus3 OneCx application.

[![License](https://img.shields.io/github/license/onecx/onecx-quarkus3-parent?style=for-the-badge&logo=apache)](https://www.apache.org/licenses/LICENSE-2.0)
[![Supported JVM Versions](https://img.shields.io/badge/JVM-17-brightgreen.svg?style=for-the-badge&logo=Java)](https://openjdk.org/projects/jdk/17/)
[![GitHub Actions Status](https://img.shields.io/github/actions/workflow/status/onecx/onecx-quarkus3-parent/build.yml?logo=GitHub&style=for-the-badge)](https://github.com/onecx/onecx-quarkus3-parent/actions/workflows/build.yml)
[![GitHub tag (latest SemVer)](https://img.shields.io/github/v/release/onecx/onecx-quarkus3-parent?display_name=tag&sort=semver&logo=github&style=for-the-badge)](https://github.com/onecx/onecx-quarkus3-parent/releases/latest)


## Versions

Branches:
* `main` - Quarkus 3.20 LTS
* `0.x` - Quarkus 3.15 LTS (deprecated)

### Definition

This parent contains:
* version of the `Quarkus 3.x.x`
* default dependencies:
    * Lombook
    * MapStruct
    * [tkit-quarkus](https://github.com/1000kit/tkit-quarkus)
    * [tkit-liquibase-plugin](https://github.com/1000kit/tkit-liquibase-plugin)
* plugin to build the application
* plugins for testing the application
* plugin to sort imports
* plugin to validate format

### Profiles

#### db-diff

To generate database diff by `liquibase` run this command
```shell
mvn clean compile -Pdb-diff
```

#### db-check

After `db-diff` run this command
```shell
mvn validate -Pdb-check
```

### How to ...

Check the [latest release](https://github.com/onecx/onecx-quarkus3-parent/releases/latest) page for details.

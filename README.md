<!-- ![CICDIcon]  -->
#  Freemarket CICD Workflows

## Description

Welcome to Freemarket centralised build and release workflows.
This repository hosts templates for a repeatable build and release process in a variety of languages and Azure resources.

## Status

<a href="https://github.com/FreemarketFX/FreemarketIaC/pulls">
  <img alt="Pull requests" src="https://img.shields.io/github/issues-pr/FreemarketFX/FreemarketIaC?color=0088ff" />
</a>


## Navigation

- [.Net Builds](#.Net-Builds)
- [Node Builds](#Parameters)
- [React Builds](#Outputs)



## .NET Builds [![.net 6](https://github.com/FreemarketFX/mockapp/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/FreemarketFX/mockapp/actions/workflows/main.yml)

<h3>Examples</h3>

<details>

<summary>Example 1</summary>

```yaml
jobs:
  dotnetbuild:
    name: 'project name - build'
    uses: reponame/build/.github/workflows/dotnetcore.yml@tags
    with:
      ProjectName: demo-api
      Projectpath: dotnetcore_Projects/MoviesAPI/MoviesAPI/*.csproj
      DotNetVersion: 6.x
      ProjectTestPath: dotnetcore_Projects/MoviesAPI/Tests/*.csproj

```

</details>

<details>

<summary>Example 2</summary>

```yaml
jobs:
  dotnetbuild:
    name: 'project name - build'
    uses: reponame/build/.github/workflows/dotnetcore.yml@tags
    with:
      ProjectName: demo-api
      Projectpath: dotnetcore_Projects/MoviesAPI/MoviesAPI/*.csproj
      DotNetVersion: 6.x
      ProjectTestPath: dotnetcore_Projects/MoviesAPI/Tests/*.csproj

```

</details>


<!-- Local -->
[CICDIcon]: docs/media/cicd.png

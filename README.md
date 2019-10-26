# SAMPLE GITVERSION DOTNET

## build

```sh
export version=$(gitversion -showvariable AssemblySemFileVer)
dotnet build /p:Version=$version /p:AssemblyVersion=$version
```

## check version

```sh
verisoninfo Domain/bin/debug/netstandard2.0/domain.dll
versioninfo webmvc/bin/debug/netcoreapp3.0/webmvc.dll
```

## show variable

```sh
gitversion
```

## show specific variable

```sh
gitversion -showvariable AssemblySemFileVer
```

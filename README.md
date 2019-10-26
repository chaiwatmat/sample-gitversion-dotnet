# SAMPLE GITVERSION DOTNET

## build

```sh
dotnet build /p:Version=$(gitversion -showvariable AssemblySemFileVer) /p:AssemblyVersion=$(gitversion -showvariable AssemblySemFileVer)
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

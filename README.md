Updated to work with latest Piranha CMS

# Flagscript.PiranhaCms.Aws.S3Storage

S3/Cloudfront Media Provider for [Piranha CMS](http://piranhacms.org).

| Version | Status |
| --- | --- |
| Latest | [![last commit](https://img.shields.io/github/last-commit/flagscript/Flagscript.PiranhaCms.Aws.S3Storage.svg?logo=github)](https://github.com/flagscript/Flagscript.PiranhaCms.Aws.S3Storage) [![build status](https://img.shields.io/appveyor/ci/Flagscript/flagscript-piranhacms-aws-s3storage.svg?logo=appveyor)](https://ci.appveyor.com/project/Flagscript/flagscript-piranhacms-aws-s3storage) [![unit test](https://img.shields.io/appveyor/tests/Flagscript/flagscript-piranhacms-aws-s3storage.svg?label=unit%20tests&logo=appveyor)](https://ci.appveyor.com/project/Flagscript/flagscript-piranhacms-aws-s3storage) |
| Master | [![last commit](https://img.shields.io/github/last-commit/flagscript/Flagscript.PiranhaCms.Aws.S3Storage/master.svg?logo=github)](https://github.com/flagscript/Flagscript.PiranhaCms.Aws.S3Storage) [![build status](https://img.shields.io/appveyor/ci/Flagscript/flagscript-piranhacms-aws-s3storage/master.svg?logo=appveyor)](https://ci.appveyor.com/project/Flagscript/flagscript-piranhacms-aws-s3storage) [![unit and integration  test](https://img.shields.io/appveyor/tests/Flagscript/flagscript-piranhacms-aws-s3storage/master.svg?label=unit/integration%20tests&logo=appveyor)](https://ci.appveyor.com/project/Flagscript/flagscript-piranhacms-aws-s3storage) [![Codacy](https://img.shields.io/codacy/grade/096a3c8d327e4e168bea4e3ebf06d402.svg?logo=codacy)](https://app.codacy.com/project/flagscript/Flagscript.PiranhaCms.Aws.S3Storage/dashboard) [![LGTM Total Alerts](https://img.shields.io/lgtm/alerts/g/flagscript/Flagscript.PiranhaCms.Aws.S3Storage.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/flagscript/Flagscript.PiranhaCms.Aws.S3Storage/alerts/) |
| Pre-Release | [![Nuget (with prereleases)](https://img.shields.io/nuget/vpre/Flagscript.PiranhaCms.Aws.S3Storage.svg?logo=nuget)](https://www.nuget.org/packages/Flagscript.PiranhaCms.Aws.S3Storage) |
| Release | [![Nuget](https://img.shields.io/nuget/v/Flagscript.PiranhaCms.Aws.S3Storage.svg?logo=nuget)](https://www.nuget.org/packages/Flagscript.PiranhaCms.Aws.S3Storage) |

## Simple Usage

The S3 File Storage for Piranha CMS operates much the same as [Local File Storage](http://piranhacms.org/docs/components/media-storage/local-file-storage) or [Azure Blob Storage](http://piranhacms.org/docs/components/media-storage/azure-blob-storage). You register S3 File Storage with the default configuration in `ConfigureServices()` with the following code:

```csharp
var storageConfig = new S3StorageConfiguration
{
	BucketName = "my-bucket-name",
	PublicUrlRoot = ""http://domain-to-my-bucket or https://my-cloudfront-bucket-distribution"
};
services.AddS3Storage(storageConfig);
```

## Documentation

[Documentation](./DOCUMENTATION.md) on how to use the Flagscript.Piranha.Aws.S3Storage library is available within this repository. 

## Download

Flagscript.PiranhaCms.Aws.S3Storage is available as a NuGet package:

### .NET CLI

```bash
> dotnet add package Flagscript.PiranhaCms.Aws.S3Storage --version 1.0.1
```

### .csproj

```xml
<PackageReference Include="Flagscript.PiranhaCms.Aws.S3Storage" Version="1.0.1" />
```
## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/flagscript/Flagscript.PiranhaCms.Aws.S3Storage/blob/master/LICENSE.md) file for details.

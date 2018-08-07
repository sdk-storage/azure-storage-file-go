# Azure Storage File SDK for Go
[![GoDoc Widget]][GoDoc] [![Build Status][Travis Widget]][Travis]

The Microsoft Azure Storage SDK for Go allows you to build applications that takes advantage of Azure's scalable cloud storage. 

This repository contains the open source File SDK for Go.

## Features
* File Storage
	* Create/List/Delete Shares
	* Create/List/Delete Directories
	* Create/Read/List/Update/Delete Files

## Getting Started
* If you don't already have it, install [the Go distribution](https://golang.org/dl/)
* Go get the SDK:

```go get github.com/Azure/azure-storage-file-go/2017-07-29/azfile```
		
## SDK Architecture

* The Azure Storage SDK for Go provides low-level and high-level APIs.
	* ServiceURL, ShareURL, DirectoryURL and FileURL objects provide the low-level API functionality and map one-to-one to the [Azure Storage File REST APIs](https://docs.microsoft.com/en-us/rest/api/storageservices/file-service-rest-api)
	* The high-level APIs provide convenience abstractions such as uploading a large stream to an Azure file (using multiple PutRange requests in parallel) or downloading a large Azure file to local (using multiple Get requests in parallel).

## Code Samples
* [File Storage Examples](https://godoc.org/github.com/Azure/azure-storage-file-go/2017-07-29/azfile#pkg-examples)

## License
This project is licensed under MIT.

## Contributing
This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

[GoDoc]: https://godoc.org/github.com/Azure/azure-storage-file-go/2017-07-29/azfile
[GoDoc Widget]: https://godoc.org/github.com/Azure/azure-storage-file-go/2017-07-29/azfile?status.svg
[Travis Widget]: https://travis-ci.org/Azure/azure-storage-file-go.svg?branch=master
[Travis]: https://travis-ci.org/Azure/azure-storage-file-go
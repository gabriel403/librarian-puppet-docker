# librarian-puppet-docker
A container for running [librarian-puppet](https://github.com/voxpupuli/librarian-puppet), by default it will install with the default configuration. 
You need to mount the volume you with for librarian-puppet to install to as `/puppet`

```
docker run -v "$PWD:/puppet" gabriel403/librarian-puppet
```
you can provide further configuration by overriding the default entry point:
```
docker run -v "$PWD:/puppet" gabriel403/librarian-puppet librarian-puppet install --verbose
```

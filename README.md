# DLOC Docker

A simple image to run [DLOC](https://github.com/SigmaInformatique/dloc)

## Licence & Copyright

Please, see the [LICENSE](https://github.com/SigmaInformatique/dloc-docker/blob/master/LICENSE) file.

## How to use it

Just run:

```
docker run -it --rm -v <your directory>:/code/ sigmainformatique/dloc
```

It will mount the directory `your directory` on the host as `/code` inside the container 

* To output the available options:

```
docker run -it --rm sigmainformatique/dloc
```

* To count lines of code in the current directory

```
docker run -it --rm -v $(pwd):/code/ sigmainformatique/dloc .
```

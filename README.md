[WeasyPrint](https://github.com/Kozea/WeasyPrint) Freezed With Docker
=====================================================================

WeasyPrint freezed onefile binary generator with pyinstaller for linux with docker.

https://docs.python-guide.org/shipping/freezing/

Usage
-----

### Build

```bash
docker build -t weasyprintfreezedwithdocker https://github.com/cakebake/WeasyPrintFreezedWithDocker.git
```

### Run

```bash
docker run -it --rm \
  -v $PWD/dist:/tmp/dist \
  --user $UID:$GID \
  weasyprintfreezedwithdocker
```

The executeable is created in `./dist/weasyprint`.

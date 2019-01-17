# A Mandelbrot Viewer

## Building and running:
```bash
$ cabal new-build
$ gpu ./run.sh
```

## Rebuilding assets:
```bash
$ cd ./resources
$ make
```

- compiling:
```bash
$ cabal new-repl exe:MandelbrotViewer
```

## Working with REPL:
- running:
```bash
$ cabal new-run exe:MandelbrotViewer
```
- with ghcid:
```bash
$ cd ${root_dir}/app
$ ghcid "--command=ghci Main.hs -i../src"
```
- alternatively, create a file `${root_dir}/app/.ghci` with the following content:
```
:set -fwarn-unused-binds -fwarn-unused-imports
:set -i../src
:load Main
```
- then we can directly call ghci, like this:
```bash
$ cd ${root_dir}/app
$ ghcid
```
## Output:
![](https://github.com/madjestic/e1337/blob/master/output.png)

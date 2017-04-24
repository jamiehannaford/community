# SIG Doc builder

This script will generate the following documentation files:

```
sig-*/README.md
sig_list.md
```

Based off the `sigs.yaml` metadata file.

## How to use 

To (re)build documentation for all the SIGs, run these commands:

```bash
docker build -t sigdocs -c build/Dockerfile build
docker run -v $(pwd):/go/src/app sigdocs
```

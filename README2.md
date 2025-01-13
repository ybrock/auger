
# start a build environnment
```
podman run -it  -v $(pwd):/go/src/github.com/etcd-io/auger:z buildauger bash

podman exec -it  buildauger bash
```

# install some tools
```
apk add bash git
```

# generate scheme.go
```
./hack/gen_scheme.sh > ./pkg/scheme/scheme.go
```

# build
```
make build
```
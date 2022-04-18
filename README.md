# starting_grpc_env

### tree
```
$ tree
.
├── README.md
├── api
│   ├── go.mod
│   └── go.sum
└── proto
    └── pancake.proto
```

### protoc exec
```
protoc --go_out=. --go_opt=paths=source_relative    --go-grpc_out=. --go-grpc_opt=paths=source_relative proto/*.proto
```
```
$ tree
.
├── README.md
├── api
│   ├── go.mod
│   └── go.sum
└── proto
    ├── pancake.pb.go
    ├── pancake.proto
    └── pancake_grpc.pb.go

2 directories, 6 files
```
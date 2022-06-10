# info
The wirelogger project repositories are currently private per the request of Seaonics

There also seems to be some issue with protobuf generation not working.
If that is the case, the following command can be used:
```
protoc --plugin=protoc-gen-ts_proto=.\node_modules\.bin\protoc-gen-ts_proto.cmd --ts_proto_out=./src --ts_proto_opt=esModuleInterop=true --ts_proto_opt=forceLong=string ./proto/<filename>.proto
```
And remember to download the [protobuf compiler binaries](https://github.com/protocolbuffers/protobuf/releases) and add them to path. The version used by the team is 3.19.4

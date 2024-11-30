**Go command to generate protos**
<!-- Assuming the command is run in root folder i.e., grpc -->
<code>protoc --go_out=server --go_opt=paths=source_relative \
    --go-grpc_out=server --go-grpc_opt=paths=source_relative \
    protos/grpc.proto</code>

<code>python3 -m grpc_tools.protoc -Iprotos --python_out=client --pyi_out=client --grpc_python_out=client protos/grpc.proto</code>
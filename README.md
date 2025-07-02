# go-concurrency-patterns

## 🕵️‍♂️ How Can We Identify a Race Condition?

To begin with, Go provides a built-in tool to detect race conditions. You can use the --race flag when compiling or running your program. This simple action will alert you if the compiler detects goroutines accessing shared variables unsafely. Early detection is crucial to avoid issues in production.

`go run -race main.go`

## Network Applications in Go

### 1. Build the Applications

```bash
# Build the chat server
go build 15-to-18-net/17-to-18-chat/chat.go

# Build the TCP client
go build 15-to-18-net/16-netcat/netcat.go
```

### 2. Run the Applications

Terminal 1 - Start the Chat Server:

```bash
./chat
```

Terminal 2 - Connect with TCP Client:

```bash
./netcat
```

Terminal 3 - Additional Client:

```bash
./netcat
```

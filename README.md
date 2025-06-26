# go-concurrency-patterns

## 🕵️‍♂️ How Can We Identify a Race Condition?

To begin with, Go provides a built-in tool to detect race conditions. You can use the --race flag when compiling or running your program. This simple action will alert you if the compiler detects goroutines accessing shared variables unsafely. Early detection is crucial to avoid issues in production.

`go go run -race main.go  `

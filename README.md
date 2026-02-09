# Go Learning Guide

A structured learning journey through Go programming, organized by concepts with corresponding code examples and detailed explanations.

## How This Guide Works

Each concept in Go is organized into:
- **Code Example**: Practical Go file in `examples/`
- **Wiki Page**: Detailed explanation, Q&A, and deep dive in the [GitHub Wiki](https://github.com/stephanie0324/learn-go/wiki)
- **Questions & Notes**: Real questions asked during learning with comprehensive answers

## Structure

```
learn-go/
├── examples/           # Go code files for each concept
│   ├── 01-hello-world.go
│   ├── 02-values.go
│   └── ...
├── go.mod             # Go module file
└── README.md          # This guide

# Detailed explanations and Q&A are in the GitHub Wiki:
# https://github.com/stephanie0324/learn-go/wiki
```

## Learning Path

### ✅ Completed Concepts

1. **[Hello World & Go Binaries](https://github.com/stephanie0324/learn-go/wiki/01-Hello-World)** (`examples/01-hello-world.go`)
   - Why Go binaries run without the Go runtime installed
   - How Go compilation differs from interpreted languages
   - Static linking and runtime bundling

2. **[Values & Basic Data Types](https://github.com/stephanie0324/learn-go/wiki/02-Values)** (`examples/02-values.go`)
   - String concatenation and operations
   - Numeric arithmetic (integers vs floats)
   - Boolean logic operations

### 🚧 Planned Concepts

3. **Variables & Types**
4. **Control Flow**
5. **Functions**
6. **Structs & Methods**
7. **Interfaces**
8. **Goroutines & Channels**
9. **Error Handling**
10. **Packages & Modules**
11. **Testing**

## How to Use This Guide

1. **Start with the code**: Look at the example in `examples/`
2. **Run the code**: Build and execute to see it in action
3. **Read the wiki**: Dive deep into the concept in the [GitHub Wiki](https://github.com/stephanie0324/learn-go/wiki)
4. **Ask questions**: Add your own questions and notes to the wiki pages
5. **Experiment**: Modify the examples to test your understanding

## Quick Start

```bash
# Clone and navigate
git clone <your-repo-url>
cd learn-go

# Run the hello world example
go run examples/01-hello-world.go

# Or build and run the binary
go build examples/01-hello-world.go
./01-hello-world
```

## Contributing to Your Own Learning

- Add new questions to existing concept pages in the [GitHub Wiki](https://github.com/stephanie0324/learn-go/wiki)
- Create new concept pages as you learn (use the wiki's "New Page" button)
- Include code snippets and examples in your wiki pages
- Document "aha!" moments and confusing points
- Reference line numbers in code when asking questions

## Learning Philosophy

This guide captures **real questions** asked during the learning process, not just textbook explanations. Each concept includes:
- The actual question that sparked curiosity
- Detailed, practical answers
- Code examples that demonstrate the concept
- Follow-up questions for deeper understanding

---

*Happy learning! 🐹*
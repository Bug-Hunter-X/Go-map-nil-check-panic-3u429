# Go Map Nil Check Panic

This repository demonstrates a common error in Go: panicking when accessing a nil map.

## The Bug

In Go, attempting to access a map that hasn't been initialized (is nil) will result in a runtime panic.  This is because the program tries to dereference a nil pointer.

The `bug.go` file shows this error.  It attempts to assign a value to a map that is not initialized, causing a panic.

## The Solution

The solution is simple. Always check if the map is nil before accessing it.   This can be achieved using a simple `if` statement. The `bugSolution.go` file demonstrates the correct way to handle this situation.

## How to Run

1. Clone this repository:
   ```bash
git clone https://github.com/YOUR_USERNAME/Go-Map-Nil-Check-Panic.git
```
2. Navigate to the directory:
   ```bash
cd Go-Map-Nil-Check-Panic
```
3. Run the buggy code (expect a panic):
   ```bash
go run bug.go
```
4. Run the corrected code:
   ```bash
go run bugSolution.go
```
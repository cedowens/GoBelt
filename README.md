# GoBelt
Golang programmatically invoking my SwiftBelt-JXA macOS system enumerator project (Golang running SwiftBelt-JXA via cgo)

## Steps
1. `go mod init gobelt/v2`
2. `go build`
3. `./gobelt`

## How This Works
This project simply leverages cgo to run Objective C Code. The Objective C code runs the embedded base64 encoded SwiftBelt-JXA.js file with the `Checks('All')` function being invoked (i.e., all SwiftBelt-JXA modules are called). This is similar to how Mythic's Poseidon golang binary invokes JXA through golang.

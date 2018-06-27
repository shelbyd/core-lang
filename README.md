# core
A language for the core of every application.

## The Problem

Writing correct software takes a large commitment to a programming language. The language often restricts where you can run the code. One essentially must write JavaScript to make a website. One often must write C/C++ to program a microcontroller. Specific systems or deployment locations often only work with specific languages.

As a result, our business logic often ends up across languages, making it difficult to see a coherent picture and work on features end-to-end.

### Our Solution

Separate out the business logic into a language that can be embedded into any deployment. Then each location, from a microcontroller to a datacenter, can share much of the same source code. The differences will only reside in how the business rules are utilized based on where they are deployed.

## What is the core?

The core is the part of applications that doesn't have anything to do with where they are run.

Some examples:
  - Entities and Use Cases in the [Clean Architecture](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html)
  - Application and Domain layers of [Hexagonal Architecture](http://fideloper.com/hexagonal-architecture)
  - Application Core of the [Onion Architecture](http://jeffreypalermo.com/blog/the-onion-architecture-part-1/)
  - Entities and Controllers in the [BCE Architecture](http://www.cs.sjsu.edu/~pearce/modules/patterns/enterprise/ecb/ecb.htm)



## Goals

### Language

- Usable and used for the core of any application
- Easy interop for other languages
- Well typed (Algebraic types)
- Obvious code
- Not be the performance bottleneck
- Writable by non-programmers
- Tests alongside code
- Clear abstractions
- Compilable or Interpretable
- Reflection to transition core-lang types to host language types

### Ecosystem

- Rapid edit-compile-test cycle
- Language agnostic core-lang test suite
- Live reloading into running applications
- Easy deployment to anything from microcontrollers to datacenters
- Allow different core programs to drop into a host architecture

## Anti-Goals

### Language

- No necessary complex constructs (lookin' at you Mondads)

### Ecosystem

- No IO

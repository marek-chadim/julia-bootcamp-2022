# Top-level

- The goal for the first session is to 
    1. familiarize people with Julia's basics
    2. demonstrate common Julia tools (VSCode, terminal, basic computer stuff)
    3. showcase a typical Julia workflow
- Roughly follow the [Julia 1.6 docs](https://docs.julialang.org/en/v1.6/)

## Pitch

I will be teaching a series of instructional Julia sessions once a month. Each month's session will be four hours of lectures, practical examples, and guided projects tailored towards economics research computing using Julia. 

Each month covers a different topic and can be attended in isolation, though the first session covers the basics of Julia and may be useful for more advanced sessions if you are not currently familiar with Julia.

Topic map:

- Julia Basics (January)
- Parallelization for Economists (Februrary)
- Optimization and Automatic Differentiation (March)
- Performant Programming and Best Practices (April)
- Bayesian Inference and Probabilistic Programming (May)

The first session is currently being held virtually via Zoom. Later sessions may be in person, circumstances permitting. 

No prior Julia experience is required, though it will be useful to have experience programming in any language.

To register, please visit =============================================

# Sketch

## Getting started

- Julia spiel, say some words about what features it has
    - Fast
    - Expressive
    - Easy
    - Pretty good package ecosystem
    - Portable
    - JIT compiled
    - Hackable
- What Julia is not (yet)
    - A smash-and-grab analysis tool (i.e. going to Julia for less than a minute or two can be counterproductive)
    - A complete substitute for old/robust tools like SAS or Stata, both of which excel at a lot of things (i.e. the GMM libraries in stata are quite good, SAS is highly optimized for streaming large data, etc.)
- Quick demo of cool things
- How to install Julia (raw binaries vs. jill?)
- How to edit Julia files (VSCode, vim, emacs, etc.)
    - Hello world!
    - Hello world for econometricians -- OLS!

## Language basics

- Variable basics
    - PRACTICE: Assignment and variable reference
- Primitive types (numerics/strings/characters)
    - Brief aside on Float/Int
- Basic operators (math/bool/etc.)
    - PRACTICE: Basic numeric operations
    - PRACTICE: String concatenation
- Array types
    - Indexing
    - Length, size, etc.
    - PRACTICE: map, broadcasting, 
    - PRACTICE: reduce
    - PRACTICE: push!, append!
    - LinearAlgebra basics
- Functions
    - returning singletons, tuples, etc.
    - Arguments
    - Keyword arguments
    - Composition/pipes
- Broadcasting!
- Control flow
    - begin
    - if
    - short-circuiting
    - while/for
    - try/catch/finally
- Scope blitz, constants
- Types
    - Abstract (briefly)
    - Composite
    - Mutable vs. immutable
    - Parametric
    - Constructors (inner vs. outer)
- Methods and multiple dispatch
- Brief section on Julia vs. R, Matlab, Python

## Package tour

- CSV and DataFrames
    - Loading data
    - How to sling data like a badass (groupby, select, filter, etc.)
    - Queryverse
- Statistics (mostly OLS, fixed effects, clustering, etc.)
    - FixedEffectModels (faster than R's felm, and Stata's reghdfe, though comparable to R feols)
    - GLM (basics mode)
    - Tables with RegressionTables.jl
- Visualization (basic plots)
    - Plots.jl
    - Makie, AlbebraOfGraphics
    - UnicodePlots.jl
- Maximum likelihood
    - Distributions.jl
    - Optim.jl

## Cool stuff

- SciML and the whole differential equations universe
    - ModelingToolkit
- Optimization
    - JuMP
    - Convex
    - Optim
- Graphs
- OnlineStats
- Math crap
    - ApproxFun
    - TaylorSeries
    - Polynomials
    - QuadGK

## Derivatives

- ChainRules
- ForwardDiff
- ReverseDiff
- FiniteDiff/FiniteDifferences
- Experimental
    - Zygote
    - Enzyme
    - Diffractor


## Bayes

- Turing
- Soss
- Stan

## Performance

- ThreadsX
- Transducers
- BangBang

## ML stuff

- MLJ
- Flux
- Clustering
- DecisionTree
- Lasso
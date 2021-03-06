# Usage

In this section we describe how to use the WorkshopWizard.

## Getting the latest workshop

To quickly get the latest workshop, install the wizard (copy-paste to Julia REPL)

```julia
] add https://github.com/crstnbr/WorkshopWizard.jl
```

and start the magic

```julia
using WorkshopWizard
WorkshopWizard.run_wizard()
```

That's it! You can now start the Jupyter notebook server and dive into the workshop materials:

```julia
using IJulia
notebook()
```

The default download path is the desktop, on windows, or the home directory, on linux/macOS.

**Note:** When running `notebook()` for the first time, IJulia might ask you whether it should install jupyter for you (because it couldn't find an existing installation). Just say yes.

## Demonstration

![wizard demo](https://raw.githubusercontent.com/crstnbr/WorkshopWizard.jl/master/demo/wizard.gif)


## Unattended installation

If you want to install the latest workshop without interactivity you can use
[`WorkshopWizard.install()`](@ref):

```@setup install
using Pkg;
pkg" add https://github.com/crstnbr/WorkshopWizard.jl/"
```

```@repl install
using WorkshopWizard
WorkshopWizard.install();
```

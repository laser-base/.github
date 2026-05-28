# Welcome to LASER!

LASER (Light Agent Spatial modeling for ERadication) is a high-performance, agent-based simulation framework for modeling the spread of infectious diseases to better inform policy decisions. It supports spatial structure, age demographics, and modular disease logic using Python-based components. LASER can also be configured to run as a compartmental model. LASER is freely available for use under the MIT license and community contributions are welcome.

## Design philosophy

The philosophy driving the development of LASER was to create a framework that was flexible, powerful, and fast, able to tackle a variety of complex modeling scenarios. But complexity often slows performance, and not every modeling question requires a full suite of model features.

To solve this, we designed LASER as a set of core components with fundamental features that could be added—or not—to build working models. You can optimize performance using only the components necessary for your modeling questions. This building-block framework enables parsimony in model design, but also facilitates the building of powerful models with bespoke, complex dynamics.

## Get started 

To get started, check out the [laser-generic docs](https://laser.idmod.org/laser-generic/), which describe how to assemble modules to create anything from simple compartmental models to more complex agent-based models with spatial dynamics for simulating the transmission of non-vector disease transmission.

If you have access to GitHub Codespaces, feel free to open the `laser-generic` repository in a Codespace (we recommend a 4-core or 8-core codespace) and run the notebooks under docs/tutorials/notebooks for yourself.

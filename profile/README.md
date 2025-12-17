# LASER disease modeling framework

The laser-base GitHub organization contains all packages for the LASER disease modeling framework. LASER (Light Agent Spatial modeling for ERadication) is a high-performance, agent-based simulation framework for modeling the spread of infectious diseases. It supports spatial structure, age demographics, and modular disease logic using Python-based components.

The philosophy driving the development of LASER was to create a framework that was flexible, powerful, and fast, able to tackle a variety of complex modeling scenarios without sacrificing performance. But complexity often slows performance, and not every modeling question requires a full suite of model features. To solve this problem, LASER was designed as a set of core components, each with fundamental features that could be added—or not—to build working models. Users can optimize performance by creating models tailored to their research needs, only using components necessary for their modeling question. This building-block framework enables parsimony in model design, but also facilitates the building of powerful models with bespoke, complex dynamics.

LASER's core principles can be summarized as follows:

- **Efficient computation**: preallocated memory, fixed-size arrays, sequential array access, and cache-friendly operations.
- **Modular design**: users define properties and add modular **components** (step functions) that run each timestep.
- **Fast**: models can be progressively optimized using **NumPy**, **Numba**, or even C/OpenMP for performance.
- **Spatial focus**: agents belong to patches (nodes), with migration modules (gravity, radiation, Stouffer’s rank, etc.) for multi-patch models.

## Documentation

Documentation for all LASER packages can be found at https://laser-base.github.io/. You may want to start with a few of our generic (SI/SIR/SEIR etc.) model explorations in the [laser-generic tutorials](https://laser-base.github.io/laser-generic/tutorials/). If you have access to GitHub Codespaces, feel free to open the `laser-generic` repository in a Codespace (we recommend a 4-core or 8-core codespace) and run the notebooks under docs/tutorials/notebooks for yourself.

## Contributions

Contributions to code or documentation to LASER packages are always welcome! See the CONTRIBUTING file in each repository for additional information.

## Disclaimer

The code in this repository was developed by IDM and other collaborators to support our joint research on flexible agent-based modeling. We've made it publicly available under the MIT License to provide others with a better understanding of our research and an opportunity to build upon it for their own work. We make no representations that the code works as intended or that we will provide support, address issues that are found, or accept pull requests. You are welcome to create your own fork and modify the code to suit your own modeling needs as permitted under the MIT License.

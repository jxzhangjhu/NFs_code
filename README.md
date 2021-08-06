# Normalizing flow implementations

<!-- ## 📦 Packages

<br> -->

## PyTorch Packages

1. [`FrEIA`](https://github.com/VLL-HD/FrEIA) by [VLL Heidelberg](https://hci.iwr.uni-heidelberg.de/vislearn) ![GitHub repo stars](https://img.shields.io/github/stars/VLL-HD/FrEIA)

    > The Framework for Easily Invertible Architectures (FrEIA) is based on RNVP flows. Easy to setup, it allows to define complex Invertible Neural Networks (INNs) from simple invertible building blocks.

2. [`nflows`](https://github.com/bayesiains/nflows) by [Bayesiains](https://homepages.inf.ed.ac.uk/imurray2/group) ![GitHub repo stars](https://img.shields.io/github/stars/bayesiains/nflows)

    > A suite of most of the SOTA methods using PyTorch. From an ML group in Edinburgh. They created the current SOTA spline flows. Almost as complete as you'll find from a single repo.

3. ['SNF'](https://github.com/noegroup/stochastic_normalizing_flows) by [Frank Noe's group](http://www.mi.fu-berlin.de/en/math/groups/ai4s)  ![GitHub repo stars](https://img.shields.io/github/stars/noegroup/stochastic_normalizing_flows)

    > They introduce sochasticity in Boltzmann-generating flows. The key methodological advance is that we avoid to compute p(x) point-wise, which would require an intractable integration over all paths mapping to the same x, and show how both training of the flow and reweighting of p(x) to exp(-u(x)) can be done via path sampling and without requiring p(x) explicitly. Part of implementation is built based on the nflows.

  4. ['Manifold-flow'](https://github.com/johannbrehmer/manifold-flow) by [Kyle Cranmer](http://theoryandpractice.org/) ![GitHub repo stars](https://img.shields.io/github/stars/johannbrehmer/manifold-flow)

      > In the paper Flows for simultaneous manifold learning and density estimation we introduce manifold-learning flows or ℳ-flows, a new class of generative models that simultaneously learn the data manifold as well as a tractable probability density on that manifold. This repository contains our implementation of ℳ-flows, as well as the code for our experiments with them.


<br>

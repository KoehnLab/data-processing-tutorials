# Motivation

Working with data can quickly become challenging if the data has one or more of the following properties
- Large, meaning there is just a lot of it
- Multidimensional
- Inhomogeneous - for example having differently structured sub-blocks or even have different blocks using different data types (e.g. dates, strings,
  numbers, etc.)

While it is usually possible to handle the data _somehow_, it typically leads to rather messy and unreadable scripts that are hard to understand
(sometimes even by the person who wrote them). This becomes even more of a problem, if multiple persons are trying to work on the same data at which
point one is often faced with the situation that every person uses different conventions and formats and most of the time those are incompatible.

Therefore, the overall aim of this tutorial is to lay some groundwork to show how such problems can be minimized by making using of existing
frameworks that allow to write data handling scripts that are easily understandable and that use the same underlying data storage format.


# Scope

The main data management package this tutorial is built on, is the [xarray](https://docs.xarray.dev/en/stable/index.html) Python package. This
tutorial is meant as an addition to the already present [xarray tutorials](https://tutorial.xarray.dev/intro.html) as well as its
[User Guide](https://docs.xarray.dev/en/stable/user-guide/index.html).

Instead of focusing on the general case, this tutorial is specifically geared towards the use case of working with data that typically comes out of
quantum chemical calculations.


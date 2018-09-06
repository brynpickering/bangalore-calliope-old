# bangalore-calliope
Calliope model, specific to a (illustrative) district in Bangalore, India

![Bangalore illustrative district](bangalore_district.pdf)

This model has been used for two papers to date. Each uses a different version of Calliope. Installation and run instructions are given below.

## 1. Mitigating risk in district-level energy investment decisions by scenario optimisation
### A.K.A. BSO2018

Paper citation: `B. Pickering, R. Choudhary. Mitigating risk in district-level energy investment decisions by scenario optimisation, In: Proceedings of the 4th IBPSA-England Conference BSO 2018, Emmanuel College, Cambridge, 2018`

### Install

This paper ran on a release candidate of Calliope 0.6.0. To install, download the `BSO2018.yml` requirements file found in the `requirements` directory of this repository. Install it by using the Calliope development environment instructions:

```shell
$ conda env create -f BSO2018.yml
```

### Running models

The notebook 'BSO2018' will guide you through building the model. As we use predefined clusters, this version of Calliope requires manually setting up the model with the full (mean demand) timeseries before editing the time dimension to match the typical days used in the modelling. You will need to install jupyter (`conda install jupyter`) into your `calliope_BSO2018` environment to directly use this notebook.

### Notes

* Native Calliope plotting will not work in most cases, due to the existence of the 'scenario' dimension.
* Since the release of Calliope 0.6.0 and subsequent releases (at the time of writing) up to 0.6.2, there have been improvements, including mathematical formulation inconsistencies. This model will be re-run once the scenario optimisation branch has been fully incorporated in a stable Calliope release.


## 2. District energy system optimisation under uncertain demand: handling data-driven stochastic profiles
### A.K.A. Decision making under uncertainty (DMUU)

Paper citation: `(Under review) B. Pickering, R. Choudhary. District energy system optimisation under uncertain demand: handling data-driven stochastic profiles, Applied Energy (2018)`

### Install

This paper ran on a development version of Calliope 0.6.2. TTo install, download the `DMUU.yml` requirements file found in the `requirements` directory of this repository. Install it by using the Calliope development environment instructions:

```shell
$ conda env create -f DMUU.yml
```

### Running models

The notebook 'DMUU' will guide you through building the model. You will need to install jupyter (`conda install jupyter`) into your `calliope_DMUU` environment to directly use this notebook.

### Notes

* Native Calliope plotting will not work in most cases, due to the existence of the 'scenario' dimension.
* This model is simpler to build than model 1, as user-defined clusters can be loaded directly into Calliope.
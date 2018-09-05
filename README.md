# bangalore-calliope
Calliope model, specific to a (illustrative) district in Bangalore, India

This model has been used for two papers to date. Each uses a different version of Calliope. Installation and run instructions are given below:

## 1. Mitigating risk in district-level energy investment decisions by scenario optimisation

Paper citation: `B. Pickering, R. Choudhary. Mitigating risk in district-level energy investment decisions by scenario optimisation, In: Proceedings of the 4th IBPSA-England Conference BSO 2018, Emmanuel College, Cambridge, 2018`

### Install

This paper ran on a release candidate of Calliope 0.6.0. To install, download the requirements file found [here](https://raw.githubusercontent.com/calliope-project/calliope/af58eb11e7bdedda221b751ad052afecff3672fc/requirements.yml). Install it by using the Calliope development environment instructions:

```shell
$ conda env create -n calliope_BSO2018 --file=requirements.yml
```

Once the environment build has completed, activate it and install pip then Calliope based on exact commit:

```shell
$ conda install pip
$ pip install git+https://github.com/calliope-project/calliope.git@af58eb11e7bdedda221b751ad052afecff3672fc
```

### Running models

The notebook 'BSO2018' will guide you through building the model. As we use predefined clusters, this version of Calliope requires manually setting up the model with the full (mean demand) timeseries before editing the time dimension to match the typical days used in the modelling.

### Notes

* Native Calliope plotting will not work in most cases, due to the existence of the 'scenario' dimension.
* Since the release of Calliope 0.6.0 and subsequent releases (at the time of writing) up to 0.6.2, there have been improvements, including mathematical formulation inconsistencies. This model will be re-run once the scenario optimisation branch has been fully incorporated in a stable Calliope release.
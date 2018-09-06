# bangalore-calliope
Calliope model, specific to a (illustrative) district in Bangalore, India.

For more information on the model structure and general use of Calliope, see [the documentation](https://calliope.readthedocs.io/en/stable/).

<object data="bangalore_district.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="bangalore_district.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://github.com/brynpickering/bangalore-calliope/blob/master/bangalore_district.pdf">Download PDF</a>.</p>
    </embed>
</object>

This model has been used for two papers to date. Each uses a different version of Calliope. Installation and run instructions are given below.

If you use this model or work derived from it in an academic publication, please cite the most recent paper in the below list.

## 1. Mitigating risk in district-level energy investment decisions by scenario optimisation
### A.K.A. BSO2018

Paper citation: `B. Pickering, R. Choudhary. Mitigating risk in district-level energy investment decisions by scenario optimisation, In: Proceedings of the 4th IBPSA-England Conference BSO 2018, Emmanuel College, Cambridge, 2018`

### Install

This paper ran on a release candidate of Calliope 0.6.0. To install, download the `BSO2018.yml` requirements file found in the `requirements` directory of this repository. Install it by using the Calliope development environment instructions:

```shell
$ conda env create -f BSO2018.yml
```

### Running models

The notebook 'BSO2018' will guide you through building the model. As we use predefined clusters, this version of Calliope requires manually setting up the model with the full (mean demand) timeseries before editing the time dimension to match the typical days used in the modelling.

### Notes

* Native Calliope plotting will not work in most cases, due to the existence of the 'scenario' dimension.
* Since the release of Calliope 0.6.0 and subsequent releases (at the time of writing) up to 0.6.2, there have been improvements, including mathematical formulation inconsistencies. This model will be re-run once the scenario optimisation branch has been fully incorporated in a stable Calliope release.


## 2. District energy system optimisation under uncertain demand: handling data-driven stochastic profiles
### A.K.A. Decision making under uncertainty (DMUU)

Paper citation: `(Under review) B. Pickering, R. Choudhary. District energy system optimisation under uncertain demand: handling data-driven stochastic profiles, Applied Energy (2018)`

### Install

This paper ran on a development version of Calliope 0.6.3. To install, download the `DMUU.yml` requirements file found in the `requirements` directory of this repository. Install it by using the Calliope development environment instructions:

```shell
$ conda env create -f DMUU.yml
```

### Running models

The notebook 'DMUU' will guide you through building the model.

### Notes

* Native Calliope plotting will not work in most cases, due to the existence of the 'scenario' dimension.
* This model is simpler to build than model 1, as user-defined clusters can be loaded directly into Calliope.

# License

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
# End-to-End Demonstration of Exp. Group B Workflow

## Summary
We are now at the stage where it is possible to conduct an end-to-end demonstration of the models and model couplings  
required for IM3 Exp. Group B experiments. This metarepository is meant to be a landing place for that
demonstration. The basic idea is that we should work off of the wiring diagram below and actually go through
the process of connecting the models together. At this stage all the component models are producing at least sample 
output datasets. Those sample outputs are sufficient for this demonstration as the purpose is to understand which 
couplings and data passes are complete and which still need more development.

<img src='experiment_diagram/experiment-B-N6_interconnect.png?raw=true' width=720 />

## Contributing models
| Model | Version | Repository Link |
|-------|---------|-----------------|
| WRF | TBD | TBD |
| Population | TBD | TBD |
| Xanthos | TBD | TBD |
| Helios | TBD | TBD |
| Persephone | TBD | TBD |
| GCAM-USA | TBD | TBD |
| TELL | v1.0 | https://github.com/IMMM-SFA/tell |
| CERF | TBD | TBD |
| GO | TBD | TBD |

## Reproduce this demonstration
1. Install the software components required to conduct the experiment from [Contributing modeling software](#contributing-modeling-software)
2. Download and install the supporting input data required to conduct the experiment from [Input data](#input-data)

| Script Name | Description | How to Run |
| --- | --- | --- |
| `step_one.py` | Script to run the first part of my experiment | `python3 step_one.py -f /path/to/inputdata/file_one.csv` |

## Reproduce the figures
Use the scripts found in the `figures` directory to reproduce the figures used in this demonstration.

| Script Name | Description | How to Run |
| --- | --- | --- |
| `generate_figures.py` | Script to generate my figures | `python3 generate_figures.py -i /path/to/inputs -o /path/to/outuptdir` |

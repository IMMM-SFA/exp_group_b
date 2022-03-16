# End-to-End Demonstration of Exp. Group B Workflow

## Summary
We are now at the stage where it is possible to conduct an end-to-end demonstration of the models and model couplings 
required for IM3 Exp. Group B experiments. This metarepository is meant to be a landing place for that
demonstration. The basic idea is that we should work off of the wiring diagram below and actually go through
the process of connecting the models together. At this stage all the component models are producing at least sample 
output datasets. Those sample outputs are sufficient for this demonstration as the purpose is to understand which 
couplings and data passes are complete and which still need more development.

<img src='experiment_diagram/experiment-B-N6_interconnect.png?raw=true' width=720 align="center" />

For the sake of the demonstration we will use the RCP 8.5 "hotter" climate forcing with the SSP5 socioeconomic
forcing: rcp85hotter_ssp5. Even if you are passing dummy or sample data from your model to a downstream model
please use this scenario name as a placeholder so that we mimic the directory structures that will be present when we  
execute the actual runs.

Please store your data for this demonstration on PNNL's Instutional Computing (PIC) at: `/pic/projects/im3/exp_group_b_test`

## Contributing models
| Model | Version | Repository Link |
|-------|---------|-----------------|
| WRF | v4.2.1 | https://github.com/IMMM-SFA/wrf_historical |
| Population | TBD | TBD |
| Xanthos | TBD | TBD |
| Helios | TBD | TBD |
| Persephone | TBD | TBD |
| GCAM-USA | TBD | TBD |
| TELL | v1.0 | https://github.com/IMMM-SFA/tell |
| CERF | TBD | TBD |
| GO | TBD | TBD |

## Forcing data
For this demonstration we'll use the IM3 WRF runs for the rcp85hotter_ssp5 scenario. Details about the forcing data 
are provided in the table below.

| Type | Platform | Years | Directory | Documentation |
|------|----------| ------| ----------| --------------|
| Climate | NERSC | 2020-2059 | /global/cfs/cdirs/m2702/gsharing/CONUS_TGW_WRF_SSP585_HOT_NEAR | https://immm-sfa.atlassian.net/wiki/spaces/IP/pages/1979809807/Accessing+Historical+and+Future+IM3+Climate+Forcing |
| Climate | NERSC | 2060-2099 | /global/cfs/cdirs/m2702/gsharing/CONUS_TGW_WRF_SSP585_HOT_FAR | https://immm-sfa.atlassian.net/wiki/spaces/IP/pages/1979809807/Accessing+Historical+and+Future+IM3+Climate+Forcing |
| Population | PIC | 2020-2100 | /pic/projects/im3/exp_group_b_test/forcing_data/population | TBD |

## Reproduce this demonstration
1. Install the software components required to conduct the experiment from [Contributing modeling software](#contributing-modeling-software)
2. Download and install the supporting input data required to conduct the experiment from [Input data](#input-data)

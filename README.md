# OpenLandMap-soildb

Production of global soil data predictions using scikit-map within the **EO-SoilMapper** framework. 
Target spatial resolution is 30 m (global coverage excluding deserts and permanent ice). 
Target period of interest is 2000 to 2022+ with 5 year intervals (spacetime block predictions). 
Depth intervals provided: 0–30, 30–60, 60–100 cm.
Predictions are based on using Quantile Regression Random Forest with with output predictions showing 
the mean plus the lower and upper prediction intervals of 68% probability to approximate one standard deviation.

This documentation is **under construction**.

## Layers available

Layers available in the current version of the OpenLandMap-soildb include:

- Soil organic carbon density [kg/m3];
- Soil organic carbon content [g/kg];
- Soil pH in H2O [-];
- Bulk density fine earth [kg/m3];
- Soil texture fraction clay-silt-sand [%];
- USDA subgroup taxa [-];

Full list of layers in available in this table. To access layers at finest resolution please use the S3 links.

For each prediction (mean value) lower and upper prediction intervals are also provided, however 
these are available only at 120 m spatial resolution.

Additional layers are available via https://stac.openlandmap.org. 

## License

[<img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" />](http://creativecommons.org/licenses/by-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

## How to cite:

To cite layers distributed via OpenLandMap-soildb please use:

- Hengl, T., Consoli, D., Tian, X., and others, (2025??). **OpenLandMap-soildb: global soil information at 30~m spatial resolution for 2000--2022+ based on spatiotemporal Machine Learning and harmonized legacy soil samples and observations**. Submitted to ESSD journal, DOI: <https://doi.org/10.5281/zenodo.4748499>.

To cite these maps please use:

```
@article{hengl_2025_essd,
  author       = {Hengl, T. and Consoli, D. and Tian, X.},
  title        = {{OpenLandMap-soildb: global soil information at 30~m spatial resolution for 2000--2022+ based on spatiotemporal Machine Learning and harmonized legacy soil samples and observations}},
  year         = 2025,
  journal    = {Earth System Science Data Discussions},
  volume      = {},
  issue       = {},
  doi          = {},
  url          = {}
}
```

## Acknowledgments

This research was supported by multiple grants, primarily by the **[Land & Carbon Lab](https://landcarbonlab.org/)** grant from the Bezos Earth Fund. The **[Open-Earth-Monitor Cyberinfrastructure](https://EarthMonitor.org)** project has received funding from the European Union's Horizon Europe research and innovation programme under grant agreement **[No. 101059548](https://cordis.europa.eu/project/id/101059548)**. **[AI4SoilHealth.eu](https://AI4SoilHealth.eu)** project has received funding from the European Union's Horizon Europe research an innovation programme under grant agreement **[No. 101086179](https://cordis.europa.eu/project/id/101086179)**. 

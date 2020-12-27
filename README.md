# redroad
Finding brick-paved alleys in Chicago

We want to use aerial imagery of Chicago to find alleys that are paved in brick.

Data Sources:

- [2019 Aerial Imagery from Cook County](https://img.cookcountyil.gov/arcgis/rest/services/Cook2019/ImageServer)

To get the source TIFFs we could automate the process

1. Walk the DownloadRasters endpoint to get the file id, ex https://img.cookcountyil.gov/arcgis/rest/services/Cook2019/ImageServer/download?rasterIds=1&geometry=&geometryType=esriGeometryEnvelope&format=&f=html
2. Get the raw file with the file endpoint: https://img.cookcountyil.gov/arcgis/rest/services/Cook2019/ImageServer/file?id=.\\Orthos2019\\RGBNIR\\01259900.tif&rasterId=1

There's about 5500 100-Mb source files, which would 550 gigabytes. I need to think about whether I want to get all the data on an external hard drive or figure out how get less data.

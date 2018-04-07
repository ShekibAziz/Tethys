1. run the file dbxmlserver.py in the folder C:\Program Files\Tethys\server

2. Run mathblab

3. Click set path and then click add with subfolders and select the following folder  C:\Program Files\Tethys\client-matlab

4. query_h = dbInit()   <-- connect to the DB (should return the following query_h = dbxml.Queries@506ad72f)

5. sample query query_h.QueryTethys(...
 'collection("SpeciesAbbreviations")/ty:Abbreviations/Name')
 =====> should return the following (<Name>NOAA.NMFS.v1</Name><Name>NOAA.NMFS.v2</Name><Name>SIO.SWAL.v1</Name>) 
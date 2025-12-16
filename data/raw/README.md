## Barrows Data
Data collected from Irish Archaeology website, downloaded in kml format from the associated Interactive Google Map, and converted to CSV. The CSV was also cleaned in Microsoft Excel to retain all downloaded information in a usable format for the sf library.

https://irisharchaeology.org/maps/

Data Dictionary for Barrows (cleaned)

| Column Name | Description | Type | Example |
|--------------|-------------|------|----------|
| townland     | Smallest land division in Ireland, of which there are ~60,000 | string | BALLINCOLLIG |
| county      | Administrative division of Ireland, of which there are 32 | string | KERRY |
| smrs      | Official Sites and Monuments Records, unique identifying number for archaeological monuments and places in Ireland, made up of letters, numbers, and dashes @archaeology.ie_2996 | string | KE030-080---- |
| entity_id | Informal identifier for the associated site, with letters and numbers | string | KE14708 |
| objectid    | Numeric identifier for sites in the Irish Archaeology database | numeric | 68203 |
| class_code      | Consise code associated with the monument_type | string | BOBA, DTBA, EMBR, MOBR, POBA, RGBA, STBA, or BARO |
| monument_type      | Classification of barrow | string | bowl barrow, ditch barrow, embanked barrow, mound barrow, pond barrow, ring-barrow, stepped barrow, or unclassified barrow |
| latitude      | Latitude coordinate of the site, in Decimal Degrees | numeric | 52.299461 |
| longitude      | Longitude coordinate of the site, in Decimal Degrees | numeric | -9.616146 |
| web_notes      | Detailed notes on the site, as written when the dataset was created  | string | Monument surveyed in 2015 and described by McGuinness (2015, 34) as following: |


https://www.archaeology.ie/app/uploads/2025/03/Archaeology-RMP-Kilkenny-Manual-1996-0022.pdf
havent figured out how to link my bib here 

Data Dictionary for Stone Circles (cleaned) (not done yet)

| Column Name | Description | Type | Example |
|--------------|-------------|------|----------|
| townland     | Smallest land division in Ireland, of which there are ~60,000 | string | BALLINCOLLIG |
| county      | Administrative division of Ireland, of which there are 32 | string | KERRY |
| smrs      | Official Sites and Monuments Records, unique identifying number for archaeological monuments and places in Ireland, made up of letters, numbers, and dashes @archaeology.ie_2996 | string | KE030-080---- |
| entity_id | Informal identifier for the associated site, with letters and numbers | string | KE14708 |
| objectid    | Numeric identifier for sites in the Irish Archaeology database | numeric | 68203 |
| class_code      | Consise code associated with the monument_type | string | BOBA, DTBA, EMBR, MOBR, POBA, RGBA, STBA, or BARO |
| monument_type      | Classification of barrow | string | bowl barrow, ditch barrow, embanked barrow, mound barrow, pond barrow, ring-barrow, stepped barrow, or unclassified barrow |
| latitude      | Latitude coordinate of the site, in Decimal Degrees | numeric | 52.299461 |
| longitude      | Longitude coordinate of the site, in Decimal Degrees | numeric | -9.616146 |
| web_notes      | Detailed notes on the site, as written when the dataset was created  | string | Monument surveyed in 2015 and described by McGuinness (2015, 34) as following: |

Note for land cover: 1990 data is called U2000_CLC1990_V2020_20u1 inside U2000_CLC1990_V2020_20u1.gdb, and 2018 is called  U2018_CLC2018_V2020_20u1 inside U2018_CLC2018_V2020_20u1.gdb

## Land Cover Data
Data came from uuhhhhh this place that I will cite eventually
Land Cover Data Classification and Reclassification

| Cell Value | CLC Code | Full Land Cover Category | New Land Cover Category | New Cell Value |
|--------------|-------------|------|----------|------|
|1	| 111	|	Artificial surfaces-Urban fabric-Continuous urban fabric | Dense Human Zones | 1 |
|2	| 112	|	Artificial surfaces-Urban fabric-Discontinuous urban fabric | Dense Human Zones | 1 |
|3	| 121	|	Artificial surfaces-Industrial, commercial and transport units-Industrial or commercial units | Dense Human Zones | 1 |
|4	| 122	|	Artificial surfaces-Industrial, commercial and transport units-Road and rail networks and associated land | Dense Human Zones | 1 |
|5	| 123	|	Artificial surfaces-Industrial, commercial and transport units-Port areas | Dense Human Zones | 1 |
|6	| 124	|	Artificial surfaces-Industrial, commercial and transport units-Airports | Dense Human Zones | 1 |
|7	| 131	|	Artificial surfaces-Mine, dump and construction sites-Mineral extraction sites | Dense Human Zones | 1 |
|8	| 132	|	Artificial surfaces-Mine, dump and construction sites-Dump sites | Dense Human Zones | 1 |
|9	| 133	|	Artificial surfaces-Mine, dump and construction sites-Construction sites | Dense Human Zones | 1 |
|10	| 141	|	Artificial surfaces-Artificial, non-agricultural vegetated areas-Green urban areas | Dense Human Zones | 1 |
|11	| 142	|	Artificial surfaces-Artificial, non-agricultural vegetated areas-Sport and leisure facilities | Dense Human Zones | 1 |
|12	| 211	|	Agricultural areas-Arable land-Non-irrigated arable land | Human Agriculture | 2 |
|13	| 212	|	Agricultural areas-Arable land-Permanently irrigated land | Human Agriculture | 2 |
|14	| 213	|	Agricultural areas-Arable land-Rice fields | Human Agriculture | 2 |
|15	| 221	|	Agricultural areas-Permanent crops-Vineyards | Human Agriculture | 2 |
|16	| 222	|	Agricultural areas-Permanent crops-Fruit trees and berry plantations | Human Agriculture | 2 |
|17	| 223	|	Agricultural areas-Permanent crops-Olive groves | Human Agriculture | 2 |
|18	| 231	|	Agricultural areas-Pastures-Pastures | Human Agriculture | 2 |
|19	| 241	|	Agricultural areas-Heterogeneous agricultural areas-Annual crops associated with permanent crops | Human Agriculture | 2 |
|20	| 242	|	Agricultural areas-Heterogeneous agricultural areas-Complex cultivation patterns | Human Agriculture | 2 |
|21	| 243	|	Agricultural areas-Heterogeneous agricultural areas-Land principally occupied by agriculture, with significant areas of natural vegetation | Human Agriculture | 2 |
|22	| 244	|	Agricultural areas-Heterogeneous agricultural areas-Agro-forestry areas | Human Agriculture | 2 |
|23	| 311	|	Forest and semi natural areas-Forests-Broad-leaved forest | Forests | 3 |
|24	| 312	|	Forest and semi natural areas-Forests-Coniferous forest | Forests | 3 |
|25	| 313	|	Forest and semi natural areas-Forests-Mixed forest | Forests | 3 |
|26	| 321	|	Forest and semi natural areas-Scrub and/or herbaceous vegetation associations-Natural grasslands | Grass and Shrublands | 4 |
|27	| 322	|	Forest and semi natural areas-Scrub and/or herbaceous vegetation associations-Moors and heathland | Grass and Shrublands | 4 |
|28	| 323	|	Forest and semi natural areas-Scrub and/or herbaceous vegetation associations-Sclerophyllous vegetation | Forests | 3 |
|29	| 324	|	Forest and semi natural areas-Scrub and/or herbaceous vegetation associations-Transitional woodland-shrub | Forests | 3 |
|30	| 331	|	Forest and semi natural areas-Open spaces with little or no vegetation-Beaches, dunes, sands | Rocky, Barren, or Snowy | 5 |
|31	| 332	|	Forest and semi natural areas-Open spaces with little or no vegetation-Bare rocks | Rocky, Barren, or Snowy | 5 |
|32	| 333	|	Forest and semi natural areas-Open spaces with little or no vegetation-Sparsely vegetated areas | Rocky, Barren, or Snowy | 5 |
|33	| 334	|	Forest and semi natural areas-Open spaces with little or no vegetation-Burnt areas | Rocky, Barren, or Snowy | 5 |
|34	| 335	|	Forest and semi natural areas-Open spaces with little or no vegetation-Glaciers and perpetual snow | Rocky, Barren, or Snowy | 5 |
|35	| 411	|	Wetlands-Inland wetlands-Inland marshes | Wetlands | 6 |
|36	| 412	|	Wetlands-Inland wetlands-Peat bogs | Wetlands | 6 |
|37	| 421	|	Wetlands-Maritime wetlands-Salt marshes | Wetlands | 6 |
|38	| 422	|	Wetlands-Maritime wetlands-Salines | Wetlands | 6 |
|39	| 423	|	Wetlands-Maritime wetlands-Intertidal flats | Wetlands | 6 |
|40	| 511	|	Water bodies-Inland waters-Water courses | Water Bodies | 7 |
|41	| 512	|	Water bodies-Inland waters-Water bodies | Water Bodies | 7 |
|42	| 521	|	Water bodies-Marine waters-Coastal lagoons | Water Bodies | 7 |
|43	| 522	|	Water bodies-Marine waters-Estuaries | Water Bodies | 7 |
|44	| 523	|	Water bodies-Marine waters-Sea and ocean | Water Bodies | 7 |
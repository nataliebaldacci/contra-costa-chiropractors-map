# Contra Costa chiropractic licensees, interactive map

Every Board of Chiropractic Examiners license with a Contra Costa County address of record (627 located so far, 497 valid), pulled from the California DCA license search (search.dca.ca.gov) on 2026-10-26 and placed on the County Assessor parcel. Click a point for the record (name, license, status, address of record, Assessor land use, APN) and a link to the DCA page.

Live map: https://nataliebaldacci.github.io/contra-costa-chiropractors-map/

- `index.html`: MapLibre GL map on the keyless OpenFreeMap "positron" style (OpenMapTiles schema, OpenStreetMap data), with the County boundary mask, city limits, County parcels and streets when zoomed in, and the County 2019 aerial (gis.cccounty.us).
- `data/licensees.geojson`: the points. Records on the same parcel are fanned out a few metres so each one can be clicked (`n_here` = how many share the parcel).
- `data/county.geojson`, `data/county_mask.geojson`, `data/cities.geojson`: Contra Costa County boundary and city limits (County GIS).

Sources: California Department of Consumer Affairs license search (Board of Chiropractic Examiners, county = Contra Costa); Contra Costa County Assessor parcel layer (CCMAP Assessment_Parcels_ArcPro) for land use and coordinates; Contra Costa County GIS for boundaries, parcels and imagery; OpenFreeMap and OpenStreetMap contributors for the base map.

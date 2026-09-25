# Richmond rooftop solar — preliminary generation estimate

A location-based screening estimate for the long western building. The 90-panel baseline remains the working option; the 85-panel alternative has lower sampled shading, but lower installed capacity. Neither layout is an installation design.

| Option | DC capacity | Modelled annual electricity | Annual daily average |
|---|---:|---:|---:|
| 90 panels | 39.6 kW | 53,670 kWh | 147.0 kWh/day |
| 85 panels | 37.4 kW | 50,688 kWh | 138.9 kWh/day |

## Basis and limitations

- European Commission JRC PVGIS 5.3, ERA5 data for 2005–2023, coordinates −37.8242866, 145.0103873.
- Crystalline-silicon modules, ventilated/free-standing mounting and 10° tilt. The service returned azimuth −172° from south, equivalent to 8° east of north; requested value was −172.3°.
- 14% system-loss input. PVGIS also models temperature/low-irradiance and angle-of-incidence effects; these are already included in the result and must not be deducted again.
- Specific production: 1,355.3 kWh per installed kW per year. Both options scale from the same 1 kW calculation; no layout-specific annual shading adjustment has been established.
- Terrain horizon enabled. This does not resolve the building’s rooftop equipment, trees, nearby buildings, or panel-to-panel shadows.
- The earlier winter geometric shade percentages are not annual electricity-loss percentages. They have NOT been deducted from these estimates.
- Inverter sizing/clipping, export limits, metering, actual self-consumption, downtime and verified structural/electrical design remain unresolved. Annual averages are not guaranteed daily output.

## Monthly output before a verified local-shading adjustment

| Month | 90 panels, kWh | 85 panels, kWh |
|---|---:|---:|
| Jan | 6,698 | 6,326 |
| Feb | 5,508 | 5,202 |
| Mar | 4,965 | 4,690 |
| Apr | 3,547 | 3,350 |
| May | 2,635 | 2,488 |
| Jun | 2,151 | 2,032 |
| Jul | 2,421 | 2,287 |
| Aug | 3,230 | 3,051 |
| Sep | 4,306 | 4,067 |
| Oct | 5,534 | 5,227 |
| Nov | 5,967 | 5,636 |
| Dec | 6,707 | 6,334 |

Monthly figures may differ slightly from annual totals because the source values are rounded.

## What it could support

Solar can contribute to common-area loads connected behind the relevant meter, particularly daytime pumps, ventilation and lift operation. Actual coverage requires interval electricity data and equipment schedules.

An illustrative lighting load—not a claim about this building—is 100 lights × 15 W × 12 hours = 18 kWh/day (6,570 kWh/year). This is only an energy comparison. If those lights run at night, direct solar cannot supply them without storage or another supply arrangement.

Do not promise that the system powers all lifts, pumps or lighting. Nameplate motor power is not annual consumption. Obtain the common-property meter bills and interval data before calculating savings, self-consumption, payback or load coverage.

## Builder-facing wording

“The 90-panel concept provides 39.6 kW of solar capacity. Preliminary location-based modelling indicates around 54 MWh of electricity annually before a verified local-shading adjustment. It could offset eligible daytime common-area electricity use, subject to site assessment, metering and detailed system design.”

## Source

[Reproducible PVGIS API request](https://re.jrc.ec.europa.eu/api/v5_3/PVcalc?lat=-37.8242866&lon=145.0103873&peakpower=1&loss=14&angle=10&aspect=-172.3&raddatabase=PVGIS-ERA5&pvtechchoice=crystSi&mountingplace=free&outputformat=json)
[PVGIS API documentation](https://joint-research-centre.ec.europa.eu/photovoltaic-geographical-information-system-pvgis/using-pvgis-5/api-non-interactive-service_en)

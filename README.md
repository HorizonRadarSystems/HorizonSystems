# Horizon Systems

A desktop-based weather radar viewing application using Qt6/C++ for various European meteorological radar networks.

Horizon Systems offers you quick access to weather radar data from various European weather services without having to use any web technology integration. This allows you to view the data with a native slippy map, radar sources support, independent split rendering, and support for custom ODIM_H5 compatible radar servers.

# How-to
Install:

sudo apt update 

sudo apt-get install -y qt6-base-dev libhdf5-dev cmake build-essential

git clone https://github.com/HorizonRadarSystems/HorizonSystems/

mkdir build && cd build

cmake .. -DCMAKE_BUILD_TYPE=Release

make -j$(nproc)

./Horizon Systems
# Features

* Native **Qt6/C++** desktop application
* Native (non-web) interactive slippy map
* Support for multiple European weather services:
  *  Deutscher Wetterdienst (DWD)
  *  Meteo-France
  * MeteoSwiss (via the EUMETNET ORD API)
  * Finnish Meteorological Institute (FMI) via its public AWS S3 bucket
* Support for custom **ODIM_H5** radar servers
* Optional custom **BUFR** API integration
* Authentication support:
  * API Key
  * OAuth2 Client Credentials
* Clickable pill-style radar site markers
* Automatic retrieval of each radar's latest available scan
* View radar data at all available elevation tilts
* Right-click anywhere on the map to enable **Split View**
  * Two completely independent radar panels
  * Independent products
  * Independent color palettes
* High-performance native rendering

# Supported Radar Networks

| Network                                | Country     | Access Method           |
| -------------------------------------- | ----------- | ----------------------- |
| Deutscher Wetterdienst (DWD)           | Germany     | Official radar services |
| Meteo-France                           | France      | Official radar services |
| MeteoSwiss                             | Switzerland | EUMETNET ORD API        |
| Finnish Meteorological Institute (FMI) | Finland     | Public AWS S3 bucket    |
| Custom Servers                         | Any         | ODIM_H5 / BUFR API      |

## Custom Radar Support

Horizon Systems can connect to your own radar applications.

Supported options include:

* ODIM_H5 serving endpoints
* BUFR APIs
* API Key authentication
* OAuth2 Client Credentials authentication

It thus qualifies the software to be used by research organizations, private radar operators, and companies exposing compatible radar systems.

# Usage

1. Launch the application.
2. Select a radar site by clicking one of the pill-shaped markers on the map.
3. The latest radar scan will be downloaded automatically.
4. Choose from any elevation tilt available for that radar.
5. Right-click the map to activate Split View for side-by-side comparison of different products or palettes.

## Technology

* C++17+
* Qt6
* Native rendering
* Native slippy map implementation
* Cross-platform desktop application

## Data Sources

Radar imagery is retrieved from official meteorological services including:

* Deutscher Wetterdienst (DWD)
* Meteo-France
* MeteoSwiss via the EUMETNET Operational Radar Data (ORD) API
* Finnish Meteorological Institute (FMI)

The application may also connect to compatible third-party ODIM_H5 or BUFR services that you configure.

## Licensing

Copyright © Horizon Radar Systems.

Developed by Ivan Dabrovich alias Perplexing, Software Engineer at Horizon Radar Systems.

Licensed under the GNU General Public License v3.0 (GPL-3.0).

Under GPL-3.0 you are free to:
* use the software
* study the source code
* modify the software
* redistribute original or modified versions
provided that redistributed versions remain licensed under GPL-3.0 and retain the original copyright notices and license text.

The full license can be found here:

https://github.com/HorizonRadarSystems/HorizonSystems#GPL-3.0-1-ov-file

### Ownership

Horizon Systems remains the original work of its authors.

Redistributing the software under GPL-3.0 does not grant permission to claim Horizon Systems, or a renamed or rebranded copy of it, as your own original work. Doing so violates both the GPL's attribution requirements and applicable copyright law. This statement is intended only as a plain-language summary of the GPL's attribution and copyleft provisions and does not alter or extend the license.

# Third-Party Data & Attribution

Horizon Systems displays third-party map tiles and weather radar data.

Please refer to:
* the attribution shown on the selected basemap,
* Deutscher Wetterdienst (DWD),
* Meteo-France,
* MeteoSwiss / EUMETNET,
* Finnish Meteorological Institute (FMI),
for their respective terms of use, licensing, attribution requirements, and data usage policies.

# Disclaimer

This software is provided as is, without warranty of any kind.

While every effort is made to accurately display meteorological radar data, Horizon Systems should not be relied upon as the sole source of information for operational, aviation, safety-critical, or life-critical decision making.
















This software is provided **as is**, without warranty of any kind.

While every effort is made to accurately display meteorological radar data, Horizon Systems should not be relied upon as the sole source of information for operational, aviation, safety-critical, or life-critical decision making.

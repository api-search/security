---
api_key_in:
- query
api_specs:
- filename: apod-openapi.yml
  format: yaml
  label: NASA Astronomy Picture of the Day (APOD)
  slug: apod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/apod-openapi.yml
- filename: asteroids-neows-openapi.yml
  format: yaml
  label: NASA Asteroids NeoWs (Near Earth Object Web Service)
  slug: asteroids-neows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/asteroids-neows-openapi.yml
- filename: donki-openapi.yml
  format: yaml
  label: NASA DONKI Space Weather API
  slug: donki
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/donki-openapi.yml
- filename: earth-openapi.yml
  format: yaml
  label: NASA Earth Imagery API
  slug: earth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/earth-openapi.yml
- filename: eonet-openapi.yml
  format: yaml
  label: NASA EONET (Earth Observatory Natural Event Tracker)
  slug: eonet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/eonet-openapi.yml
- filename: epic-openapi.yml
  format: yaml
  label: NASA EPIC (Earth Polychromatic Imaging Camera)
  slug: epic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/epic-openapi.yml
- filename: exoplanet-openapi.yml
  format: yaml
  label: NASA Exoplanet Archive API
  slug: exoplanet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/exoplanet-openapi.yml
- filename: insight-openapi.yml
  format: yaml
  label: NASA InSight Mars Weather Service API
  slug: insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/insight-openapi.yml
- filename: mars-rover-photos-openapi.yml
  format: yaml
  label: NASA Mars Rover Photos API
  slug: mars-rover-photos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/mars-rover-photos-openapi.yml
- filename: image-video-library-openapi.yml
  format: yaml
  label: NASA Image and Video Library API
  slug: image-video-library
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/image-video-library-openapi.yml
- filename: techtransfer-openapi.yml
  format: yaml
  label: NASA TechTransfer API
  slug: techtransfer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/techtransfer-openapi.yml
- filename: ssd-cneos-openapi.yml
  format: yaml
  label: NASA SSD/CNEOS API
  slug: ssd-cneos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/ssd-cneos-openapi.yml
- filename: techport-openapi.yml
  format: yaml
  label: NASA TechPort API
  slug: techport
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/techport-openapi.yml
- filename: tle-openapi.yml
  format: yaml
  label: NASA TLE API (Two-Line Element Set)
  slug: tle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/tle-openapi.yml
- filename: satellite-situation-center-openapi.yml
  format: yaml
  label: NASA Satellite Situation Center API
  slug: satellite-situation-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/satellite-situation-center-openapi.yml
- filename: genelab-openapi.yml
  format: yaml
  label: NASA GeneLab Search API
  slug: genelab
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/genelab-openapi.yml
- filename: trek-wmts-openapi.yml
  format: yaml
  label: NASA Vesta/Moon/Mars Trek WMTS
  slug: trek-wmts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/trek-wmts-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nasa Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: NASA Open APIs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NASA Open APIs
provider_slug: nasa-gov
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/apod-openapi.yml
  - openapi/asteroids-neows-openapi.yml
  - openapi/donki-openapi.yml
  - openapi/earth-openapi.yml
  - openapi/epic-openapi.yml
  - openapi/insight-openapi.yml
  - openapi/mars-rover-photos-openapi.yml
  - openapi/techport-openapi.yml
  - openapi/techtransfer-openapi.yml
  type: apiKey
slug: nasa-gov-authentication
source_filename: nasa-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apod-openapi.yml, openapi/asteroids-neows-openapi.yml, openapi/donki-openapi.yml,\n  openapi/earth-openapi.yml, openapi/epic-openapi.yml, openapi/insight-openapi.yml, openapi/mars-rover-photos-openapi.yml,\n  openapi/techport-openapi.yml, openapi/techtransfer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/apod-openapi.yml\n  - openapi/asteroids-neows-openapi.yml\n  - openapi/donki-openapi.yml\n  - openapi/earth-openapi.yml\n  - openapi/epic-openapi.yml\n  - openapi/insight-openapi.yml\n  - openapi/mars-rover-photos-openapi.yml\n  - openapi/techport-openapi.yml\n  - openapi/techtransfer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/authentication/nasa-gov-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Federal
- Space
- Earth Science
- Open Data
- Astronomy
- Planetary Science
- Heliophysics
- Bioscience
- NASA
---

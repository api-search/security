---
api_key_in:
- header
- query
api_specs:
- filename: aeso-aiesgencapacity-api-openapi.yml
  format: yaml
  label: AESO AIES Gen Capacity API
  slug: aeso-aiesgencapacity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-aiesgencapacity-api-openapi.yml
- filename: aeso-assetlist-api-openapi.yml
  format: yaml
  label: AESO Assetlist API
  slug: aeso-assetlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-assetlist-api-openapi.yml
- filename: aeso-csd-api-openapi.yml
  format: yaml
  label: AESO Csd API
  slug: aeso-csd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-csd-api-openapi.yml
- filename: aeso-interchange-api-openapi.yml
  format: yaml
  label: AESO Interchange API
  slug: aeso-interchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-interchange-api-openapi.yml
- filename: aeso-load-api-openapi.yml
  format: yaml
  label: AESO Load API
  slug: aeso-load-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-load-api-openapi.yml
- filename: aeso-loadoutagereport-api-openapi.yml
  format: yaml
  label: AESO Load Outage Report API
  slug: aeso-loadoutagereport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-loadoutagereport-api-openapi.yml
- filename: aeso-meritorder-api-openapi.yml
  format: yaml
  label: AESO Merit Order API
  slug: aeso-meritorder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-meritorder-api-openapi.yml
- filename: aeso-meteredvolume-api-openapi.yml
  format: yaml
  label: AESO Meteredvolume API
  slug: aeso-meteredvolume-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-meteredvolume-api-openapi.yml
- filename: aeso-operatingreserveoffercontrol-api-openapi.yml
  format: yaml
  label: AESO Operating Reserve Offer Control API
  slug: aeso-operatingreserveoffercontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-operatingreserveoffercontrol-api-openapi.yml
- filename: aeso-outage-api-openapi.yml
  format: yaml
  label: AESO Outage API
  slug: aeso-outage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-outage-api-openapi.yml
- filename: aeso-poolparticipantlist-api-openapi.yml
  format: yaml
  label: AESO Poolparticipantlist API
  slug: aeso-poolparticipantlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-poolparticipantlist-api-openapi.yml
- filename: aeso-price-api-openapi.yml
  format: yaml
  label: AESO Price API
  slug: aeso-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-price-api-openapi.yml
- filename: aeso-unitcommitment-api-openapi.yml
  format: yaml
  label: AESO Unit Commitment API
  slug: aeso-unitcommitment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-unitcommitment-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aeso Authentication
name_suffix: Authentication
oauth_flows: []
overview: AESO secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AESO
provider_slug: aeso
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: API-KEY
  sources:
  - openapi/aeso-actualforecast-api-v1-openapi.json
  - openapi/aeso-aiesgencapacity-api-v1-openapi.json
  - openapi/aeso-assetlist-api-v1-openapi.json
  - openapi/aeso-currentsupplydemand-api-v1-openapi.json
  - openapi/aeso-currentsupplydemand-api-v2-openapi.json
  - openapi/aeso-energymeritorder-api-v1-openapi.json
  - openapi/aeso-itc-api-v1-openapi.json
  - openapi/aeso-loadoutageforecast-api-v1-openapi.json
  - openapi/aeso-meteredvolume-api-v1-openapi.json
  - openapi/aeso-operatingreserveoffercontrol-api-v1-openapi.json
  - openapi/aeso-poolparticipant-api-v1-openapi.json
  - openapi/aeso-poolprice-api-v1-1-openapi.json
  - openapi/aeso-systemmarginalprice-api-v1-1-openapi.json
  - openapi/aeso-unitcommitmentdata-api-v2-openapi.json
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/aeso-actualforecast-api-v1-openapi.json
  - openapi/aeso-aiesgencapacity-api-v1-openapi.json
  - openapi/aeso-assetlist-api-v1-openapi.json
  - openapi/aeso-currentsupplydemand-api-v1-openapi.json
  - openapi/aeso-currentsupplydemand-api-v2-openapi.json
  - openapi/aeso-energymeritorder-api-v1-openapi.json
  - openapi/aeso-itc-api-v1-openapi.json
  - openapi/aeso-loadoutageforecast-api-v1-openapi.json
  - openapi/aeso-meteredvolume-api-v1-openapi.json
  - openapi/aeso-operatingreserveoffercontrol-api-v1-openapi.json
  - openapi/aeso-poolparticipant-api-v1-openapi.json
  - openapi/aeso-poolprice-api-v1-1-openapi.json
  - openapi/aeso-systemmarginalprice-api-v1-1-openapi.json
  - openapi/aeso-unitcommitmentdata-api-v2-openapi.json
  type: apiKey
slug: aeso-authentication
source_filename: aeso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/aeso-actualforecast-api-v1-openapi.json, openapi/aeso-aiesgencapacity-api-v1-openapi.json,\n  openapi/aeso-assetlist-api-v1-openapi.json, openapi/aeso-currentsupplydemand-api-v1-openapi.json,\n  openapi/aeso-currentsupplydemand-api-v2-openapi.json, openapi/aeso-energymeritorder-api-v1-openapi.json,\n  openapi/aeso-itc-api-v1-openapi.json, openapi/aeso-loadoutageforecast-api-v1-openapi.json,\n  openapi/aeso-meteredvolume-api-v1-openapi.json, openapi/aeso-operatingreserveoffercontrol-api-v1-openapi.json,\n  openapi/aeso-poolparticipant-api-v1-openapi.json, openapi/aeso-poolprice-api-v1-1-openapi.json\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: API-KEY\n  sources:\n  - openapi/aeso-actualforecast-api-v1-openapi.json\n  - openapi/aeso-aiesgencapacity-api-v1-openapi.json\n  - openapi/aeso-assetlist-api-v1-openapi.json\n\
  \  - openapi/aeso-currentsupplydemand-api-v1-openapi.json\n  - openapi/aeso-currentsupplydemand-api-v2-openapi.json\n  - openapi/aeso-energymeritorder-api-v1-openapi.json\n  - openapi/aeso-itc-api-v1-openapi.json\n  - openapi/aeso-loadoutageforecast-api-v1-openapi.json\n  - openapi/aeso-meteredvolume-api-v1-openapi.json\n  - openapi/aeso-operatingreserveoffercontrol-api-v1-openapi.json\n  - openapi/aeso-poolparticipant-api-v1-openapi.json\n  - openapi/aeso-poolprice-api-v1-1-openapi.json\n  - openapi/aeso-systemmarginalprice-api-v1-1-openapi.json\n  - openapi/aeso-unitcommitmentdata-api-v2-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/aeso-actualforecast-api-v1-openapi.json\n  - openapi/aeso-aiesgencapacity-api-v1-openapi.json\n  - openapi/aeso-assetlist-api-v1-openapi.json\n  - openapi/aeso-currentsupplydemand-api-v1-openapi.json\n  - openapi/aeso-currentsupplydemand-api-v2-openapi.json\n  - openapi/aeso-energymeritorder-api-v1-openapi.json\n\
  \  - openapi/aeso-itc-api-v1-openapi.json\n  - openapi/aeso-loadoutageforecast-api-v1-openapi.json\n  - openapi/aeso-meteredvolume-api-v1-openapi.json\n  - openapi/aeso-operatingreserveoffercontrol-api-v1-openapi.json\n  - openapi/aeso-poolparticipant-api-v1-openapi.json\n  - openapi/aeso-poolprice-api-v1-1-openapi.json\n  - openapi/aeso-systemmarginalprice-api-v1-1-openapi.json\n  - openapi/aeso-unitcommitmentdata-api-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/authentication/aeso-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Energy
- Canada
- Alberta
- Electricity
- Energy Markets
- Grid
- System Operator
- Market Operator
- Open Energy Data
- Wholesale Power
- Demand Response
- Renewables
- Utilities
---

---
api_key_in:
- header
- query
api_specs:
- filename: aeso-poolprice-api-v1-1-openapi.json
  format: json
  label: AESO Pool Price Report API
  slug: aeso-pool-price-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-poolprice-api-v1-1-openapi.json
- filename: aeso-systemmarginalprice-api-v1-1-openapi.json
  format: json
  label: AESO System Marginal Price Report API
  slug: aeso-system-marginal-price-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-systemmarginalprice-api-v1-1-openapi.json
- filename: aeso-currentsupplydemand-api-v2-openapi.json
  format: json
  label: AESO Current Supply Demand API (v2)
  slug: aeso-current-supply-demand-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-currentsupplydemand-api-v2-openapi.json
- filename: aeso-currentsupplydemand-api-v1-openapi.json
  format: json
  label: AESO Current Supply Demand API (v1)
  slug: aeso-current-supply-demand-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-currentsupplydemand-api-v1-openapi.json
- filename: aeso-actualforecast-api-v1-openapi.json
  format: json
  label: AESO Actual Forecast Report API
  slug: aeso-actual-forecast-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-actualforecast-api-v1-openapi.json
- filename: aeso-aiesgencapacity-api-v1-openapi.json
  format: json
  label: AESO AIES Gen Capacity API
  slug: aeso-aies-gen-capacity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-aiesgencapacity-api-v1-openapi.json
- filename: aeso-loadoutageforecast-api-v1-openapi.json
  format: json
  label: AESO Load Outage Forecast API
  slug: aeso-load-outage-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-loadoutageforecast-api-v1-openapi.json
- filename: aeso-itc-api-v1-openapi.json
  format: json
  label: AESO Intertie Public Reports API
  slug: aeso-intertie-public-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-itc-api-v1-openapi.json
- filename: aeso-energymeritorder-api-v1-openapi.json
  format: json
  label: AESO Energy Merit Order Report API
  slug: aeso-energy-merit-order-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-energymeritorder-api-v1-openapi.json
- filename: aeso-meteredvolume-api-v1-openapi.json
  format: json
  label: AESO Metered Volume Report API
  slug: aeso-metered-volume-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-meteredvolume-api-v1-openapi.json
- filename: aeso-operatingreserveoffercontrol-api-v1-openapi.json
  format: json
  label: AESO Operating Reserve Offer Control Report API
  slug: aeso-operating-reserve-offer-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-operatingreserveoffercontrol-api-v1-openapi.json
- filename: aeso-assetlist-api-v1-openapi.json
  format: json
  label: AESO Asset List API
  slug: aeso-asset-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-assetlist-api-v1-openapi.json
- filename: aeso-poolparticipant-api-v1-openapi.json
  format: json
  label: AESO Pool Participant API
  slug: aeso-pool-participant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-poolparticipant-api-v1-openapi.json
- filename: aeso-unitcommitmentdata-api-v2-openapi.json
  format: json
  label: AESO Unit Commitment Data API
  slug: aeso-unit-commitment-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-unitcommitmentdata-api-v2-openapi.json
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

---
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
description: ''
domains:
- caa:
  - 0 issue "starfieldtech.com"
  - 0 issue "ssl.com"
  - 0 issuewild "ssl.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aeso.ca
  spf: true
hosts:
- cert_expires: Sep  5 19:55:02 2026 GMT
  host: www.aeso.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: developer-apim.aeso.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: apimgw.aeso.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aeso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AESO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AESO
provider_slug: aeso
slug: aeso-domain-security
source_filename: aeso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeso.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:55:02 2026 GMT\n  hsts: false\n- host: developer-apim.aeso.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apimgw.aeso.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: aeso.ca\n  dnssec: false\n  caa:\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/security/aeso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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

---
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

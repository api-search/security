---
api_specs:
- filename: bridge-mls-agents-api-openapi.yml
  format: yaml
  label: Bridge Agents API
  slug: bridge-mls-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-agents-api-openapi.yml
- filename: bridge-mls-listings-api-openapi.yml
  format: yaml
  label: Bridge Listings API
  slug: bridge-mls-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-listings-api-openapi.yml
- filename: bridge-mls-media-api-openapi.yml
  format: yaml
  label: Bridge Media API
  slug: bridge-mls-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-media-api-openapi.yml
- filename: bridge-mls-member-api-openapi.yml
  format: yaml
  label: Bridge Member API
  slug: bridge-mls-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-member-api-openapi.yml
- filename: bridge-mls-metadata-api-openapi.yml
  format: yaml
  label: Bridge Metadata API
  slug: bridge-mls-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-metadata-api-openapi.yml
- filename: bridge-mls-office-api-openapi.yml
  format: yaml
  label: Bridge Office API
  slug: bridge-mls-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-office-api-openapi.yml
- filename: bridge-mls-offices-api-openapi.yml
  format: yaml
  label: Bridge Offices API
  slug: bridge-mls-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-offices-api-openapi.yml
- filename: bridge-mls-openhouse-api-openapi.yml
  format: yaml
  label: Bridge OpenHouse API
  slug: bridge-mls-openhouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-openhouse-api-openapi.yml
- filename: bridge-mls-openhouses-api-openapi.yml
  format: yaml
  label: Bridge OpenHouses API
  slug: bridge-mls-openhouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-openhouses-api-openapi.yml
- filename: bridge-mls-property-api-openapi.yml
  format: yaml
  label: Bridge Property API
  slug: bridge-mls-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-property-api-openapi.yml
- filename: bridge-mls-webhooks-api-openapi.yml
  format: yaml
  label: Bridge Webhooks API
  slug: bridge-mls-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bridgeinteractive.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bridgedataoutput.com
  spf: false
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: www.bridgeinteractive.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: bridgedataoutput.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.bridgedataoutput.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bridge Mls Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridge, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bridge
provider_slug: bridge-mls
slug: bridge-mls-domain-security
source_filename: bridge-mls-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bridgeinteractive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: bridgedataoutput.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bridgedataoutput.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bridgeinteractive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bridgedataoutput.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/security/bridge-mls-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- MLS
- RESO
- Listings
- Property Data
- Brokers
- Data Distribution
---

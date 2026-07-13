---
api_specs:
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Listings and Properties API
  slug: listings-properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Agents API
  slug: agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Offices API
  slug: offices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Open Houses API
  slug: open-houses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge RESO Web API
  slug: reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
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
name: Bridge Interactive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridge Interactive, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bridge Interactive
provider_slug: bridge-interactive
slug: bridge-interactive-domain-security
source_filename: bridge-interactive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bridgeinteractive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: bridgedataoutput.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bridgedataoutput.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bridgeinteractive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bridgedataoutput.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/security/bridge-interactive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- MLS
- RESO
- Listings
- Property Data
---

---
api_specs:
- filename: uk-power-networks-explore-api-v2-1-openapi.json
  format: json
  label: UK Power Networks Open Data Explore API v2.1
  slug: uk-power-networks-explore-api-v2-1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/openapi/uk-power-networks-explore-api-v2-1-openapi.json
- filename: uk-power-networks-explore-api-v2-0-openapi.json
  format: json
  label: UK Power Networks Open Data Explore API v2.0
  slug: uk-power-networks-explore-api-v2-0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/openapi/uk-power-networks-explore-api-v2-0-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ukpowernetworks.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opendatasoft.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.ukpowernetworks.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 21:02:03 2026 GMT
  host: ukpowernetworks.opendatasoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uk Power Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UK Power Networks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UK Power Networks
provider_slug: uk-power-networks
slug: uk-power-networks-domain-security
source_filename: uk-power-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ukpowernetworks.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\n- host: ukpowernetworks.opendatasoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ukpowernetworks.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: opendatasoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/security/uk-power-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- Smart Metering
- DER
- EV Charging
- Carbon
- Energy Markets
---

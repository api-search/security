---
api_specs:
- filename: electricity-north-west-catalog-api-openapi.yml
  format: yaml
  label: Electricity North West Catalog API
  slug: electricity-north-west-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/openapi/electricity-north-west-catalog-api-openapi.yml
- filename: electricity-north-west-dataset-api-openapi.yml
  format: yaml
  label: Electricity North West Dataset API
  slug: electricity-north-west-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/openapi/electricity-north-west-dataset-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: enwl.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opendatasoft.com
  spf: true
hosts:
- cert_expires: Sep 21 18:15:34 2026 GMT
  host: www.enwl.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 21:02:03 2026 GMT
  host: electricitynorthwest.opendatasoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Electricity North West Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electricity North West, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Electricity North West
provider_slug: electricity-north-west
slug: electricity-north-west-domain-security
source_filename: electricity-north-west-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enwl.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:15:34 2026 GMT\n  hsts: null\n- host: electricitynorthwest.opendatasoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: enwl.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: opendatasoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/security/electricity-north-west-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- DER
- Renewables
- Energy Markets
- Smart Metering
---

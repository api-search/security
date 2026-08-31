---
api_specs:
- filename: scottishpower-catalog-api-openapi.yml
  format: yaml
  label: ScottishPower Catalog API
  slug: scottishpower-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scottishpower/refs/heads/main/openapi/scottishpower-catalog-api-openapi.yml
- filename: scottishpower-dataset-api-openapi.yml
  format: yaml
  label: ScottishPower Dataset API
  slug: scottishpower-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scottishpower/refs/heads/main/openapi/scottishpower-dataset-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scottishpower.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spenergynetworks.co.uk
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.scottishpower.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.spenergynetworks.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 21:02:03 2026 GMT
  host: spenergynetworks.opendatasoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scottishpower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScottishPower, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ScottishPower
provider_slug: scottishpower
slug: scottishpower-domain-security
source_filename: scottishpower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scottishpower.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\n- host: www.spenergynetworks.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\n- host: spenergynetworks.opendatasoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scottishpower.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spenergynetworks.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scottishpower/refs/heads/main/security/scottishpower-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Retailer
- Smart Metering
- Grid
- Open Data
- Distribution Network Operator
- Renewables
- Energy Markets
---

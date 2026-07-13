---
api_specs:
- filename: redfin-stingray-api-openapi.yml
  format: yaml
  label: Redfin Stingray API
  slug: redfin-stingray-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-stingray-api-openapi.yml
- filename: redfin-gis-csv-api-openapi.yml
  format: yaml
  label: Redfin GIS CSV Export API
  slug: redfin-gis-csv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-gis-csv-api-openapi.yml
- filename: redfin-data-center-openapi.yml
  format: yaml
  label: Redfin Data Center
  slug: redfin-data-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-data-center-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: redfin.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.redfin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: redfin-public-data.s3.us-west-2.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redfin, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Redfin
provider_slug: redfin
slug: redfin-domain-security
source_filename: redfin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redfin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\n- host: redfin-public-data.s3.us-west-2.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: redfin.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/security/redfin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CSV Export
- GIS
- Home Values
- Housing Market
- Listings
- Property Data
- Real Estate
---

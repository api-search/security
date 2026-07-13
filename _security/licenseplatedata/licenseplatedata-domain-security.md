---
api_specs:
- filename: licenseplatedata-openapi.yml
  format: yaml
  label: LicensePlateData
  slug: licenseplatedata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/licenseplatedata/refs/heads/main/openapi/licenseplatedata-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: licenseplatedata.com
  spf: true
hosts:
- cert_expires: Aug 16 17:18:29 2026 GMT
  host: licenseplatedata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 17:18:29 2026 GMT
  host: api.licenseplatedata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Licenseplatedata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LicensePlateData, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LicensePlateData
provider_slug: licenseplatedata
slug: licenseplatedata-domain-security
source_filename: licenseplatedata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: licenseplatedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:18:29 2026 GMT\n  hsts: false\n- host: api.licenseplatedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:18:29 2026 GMT\n  hsts: null\ndomains:\n- domain: licenseplatedata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/licenseplatedata/refs/heads/main/security/licenseplatedata-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vehicles
- License Plates
- VIN
- Automotive
- Plate Lookup
- VIN Decoding
---

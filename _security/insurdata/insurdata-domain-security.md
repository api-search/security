---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: insurdata.io
  spf: false
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.insurdata.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insurdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insurdata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Insurdata
provider_slug: insurdata
slug: insurdata-domain-security
source_filename: insurdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.insurdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: insurdata.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insurdata/refs/heads/main/security/insurdata-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Insurance
- Reinsurance
- Geocoding
- Exposure Data
- Property Data
- Risk
- Catastrophe Modeling
- Insurtech
- Geospatial
---

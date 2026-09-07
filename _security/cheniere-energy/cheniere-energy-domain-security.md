---
api_specs:
- filename: cheniere-energy-lng-connection.yml
  format: yaml
  label: Cheniere LNG Connection Pipeline Informational Postings API
  slug: lng-connection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-lng-connection.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cheniere.com
  spf: true
hosts:
- cert_expires: Nov 15 08:05:24 2026 GMT
  host: www.cheniere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: lngconnection.cheniere.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: lngconnectionapi.cheniere.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cheniere Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cheniere Energy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cheniere Energy
provider_slug: cheniere-energy
slug: cheniere-energy-domain-security
source_filename: cheniere-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cheniere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 08:05:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: lngconnection.cheniere.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: lngconnectionapi.cheniere.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cheniere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/security/cheniere-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corpus Christi
- Energy
- Export
- FERC
- Houston
- Informational Postings
- LNG
- Liquefaction
- NAESB
- Natural Gas
- Open Data
- Pipelines
- Regasification
- Sabine Pass
- Texas
---

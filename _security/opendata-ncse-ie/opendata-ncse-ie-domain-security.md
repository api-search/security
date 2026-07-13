---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ncse.ie
  spf: true
hosts:
- cert_expires: Oct  2 06:56:55 2026 GMT
  host: opendata.ncse.ie
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Ncse Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NCSE Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NCSE Open Data
provider_slug: opendata-ncse-ie
slug: opendata-ncse-ie-domain-security
source_filename: opendata-ncse-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.ncse.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:56:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ncse.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-ncse-ie/refs/heads/main/security/opendata-ncse-ie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Government Agency
- Ireland
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bz.it
  spf: false
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: data.civis.bz.it
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data Civis Bz It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for South Tyrol Civis Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: South Tyrol Civis Open Data
provider_slug: data-civis-bz-it
slug: data-civis-bz-it-domain-security
source_filename: data-civis-bz-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.civis.bz.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: bz.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-civis-bz-it/refs/heads/main/security/data-civis-bz-it-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- Italy
---

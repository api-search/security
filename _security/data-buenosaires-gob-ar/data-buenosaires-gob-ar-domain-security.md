---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gob.ar
  spf: false
hosts:
- cert_expires: Apr  4 23:59:59 2027 GMT
  host: data.buenosaires.gob.ar
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data Buenosaires Gob Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buenos Aires Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Buenos Aires Data
provider_slug: data-buenosaires-gob-ar
slug: data-buenosaires-gob-ar-domain-security
source_filename: data-buenosaires-gob-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.buenosaires.gob.ar\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gob.ar\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-buenosaires-gob-ar/refs/heads/main/security/data-buenosaires-gob-ar-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Argentina
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gob.ar
  spf: false
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: datos.magyp.gob.ar
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datos Magyp Gob Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datos Agricultura Argentina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Datos Agricultura Argentina
provider_slug: datos-magyp-gob-ar
slug: datos-magyp-gob-ar-domain-security
source_filename: datos-magyp-gob-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.magyp.gob.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gob.ar\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datos-magyp-gob-ar/refs/heads/main/security/datos-magyp-gob-ar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Government Agency
- Argentina
---

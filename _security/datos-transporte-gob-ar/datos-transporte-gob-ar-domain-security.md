---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gob.ar
  spf: false
hosts:
- cert_expires: Sep 24 16:50:21 2026 GMT
  host: datos.transporte.gob.ar
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Datos Transporte Gob Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datos Transporte Argentina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Datos Transporte Argentina
provider_slug: datos-transporte-gob-ar
slug: datos-transporte-gob-ar-domain-security
source_filename: datos-transporte-gob-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.transporte.gob.ar\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 16:50:21 2026 GMT\n  hsts: false\ndomains:\n- domain: gob.ar\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datos-transporte-gob-ar/refs/heads/main/security/datos-transporte-gob-ar-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Government Agency
- Argentina
---

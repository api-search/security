---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gob.do
  spf: false
hosts:
- cert_expires: Aug 22 00:03:27 2026 GMT
  host: datos.gob.do
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datos Gob Do Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portal de Datos Abiertos Republica Dominicana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Portal de Datos Abiertos Republica Dominicana
provider_slug: datos-gob-do
slug: datos-gob-do-domain-security
source_filename: datos-gob-do-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.gob.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 00:03:27 2026 GMT\n  hsts: false\ndomains:\n- domain: gob.do\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datos-gob-do/refs/heads/main/security/datos-gob-do-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Dominican Republic
---

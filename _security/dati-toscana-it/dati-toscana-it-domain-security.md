---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: toscana.it
  spf: false
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: dati.toscana.it
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dati Toscana It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Data Regione Toscana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Data Regione Toscana
provider_slug: dati-toscana-it
slug: dati-toscana-it-domain-security
source_filename: dati-toscana-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.toscana.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: toscana.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-toscana-it/refs/heads/main/security/dati-toscana-it-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Italy
---

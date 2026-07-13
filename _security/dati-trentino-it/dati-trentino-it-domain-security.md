---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trentino.it
  spf: false
hosts:
- cert_expires: Mar  7 09:58:41 2027 GMT
  host: dati.trentino.it
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dati Trentino It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Data Trentino, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Data Trentino
provider_slug: dati-trentino-it
slug: dati-trentino-it-domain-security
source_filename: dati-trentino-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.trentino.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 09:58:41 2027 GMT\n  hsts: false\ndomains:\n- domain: trentino.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-trentino-it/refs/heads/main/security/dati-trentino-it-domain-security.yml
summary_line: TLSv1.2
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Italy
---

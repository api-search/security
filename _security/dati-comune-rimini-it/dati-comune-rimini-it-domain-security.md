---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rimini.it
  spf: false
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: dati.comune.rimini.it
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dati Comune Rimini It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rimini Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rimini Open Data
provider_slug: dati-comune-rimini-it
slug: dati-comune-rimini-it-domain-security
source_filename: dati-comune-rimini-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.comune.rimini.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rimini.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-comune-rimini-it/refs/heads/main/security/dati-comune-rimini-it-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Italy
---

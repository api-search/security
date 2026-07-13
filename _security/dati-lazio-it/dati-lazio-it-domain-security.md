---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lazio.it
  spf: false
hosts:
- cert_expires: Oct 25 11:26:14 2026 GMT
  host: dati.lazio.it
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dati Lazio It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lazio Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lazio Open Data
provider_slug: dati-lazio-it
slug: dati-lazio-it-domain-security
source_filename: dati-lazio-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.lazio.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 11:26:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: lazio.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-lazio-it/refs/heads/main/security/dati-lazio-it-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- Italy
---

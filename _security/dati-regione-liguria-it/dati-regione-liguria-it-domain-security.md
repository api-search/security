---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: liguria.it
  spf: false
hosts:
- cert_expires: Oct 14 12:28:54 2026 GMT
  host: dati.regione.liguria.it
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dati Regione Liguria It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liguria Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Liguria Open Data
provider_slug: dati-regione-liguria-it
slug: dati-regione-liguria-it-domain-security
source_filename: dati-regione-liguria-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.regione.liguria.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:28:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: liguria.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-regione-liguria-it/refs/heads/main/security/dati-regione-liguria-it-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Regional Government
- Italy
---

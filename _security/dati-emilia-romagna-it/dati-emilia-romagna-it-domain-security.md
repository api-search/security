---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: emilia-romagna.it
  spf: false
hosts:
- cert_expires: Aug 24 16:57:54 2026 GMT
  host: dati.emilia-romagna.it
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dati Emilia Romagna It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dati.emilia-romagna.it, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: dati.emilia-romagna.it
provider_slug: dati-emilia-romagna-it
slug: dati-emilia-romagna-it-domain-security
source_filename: dati-emilia-romagna-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.emilia-romagna.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 16:57:54 2026 GMT\n  hsts: null\ndomains:\n- domain: emilia-romagna.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-emilia-romagna-it/refs/heads/main/security/dati-emilia-romagna-it-domain-security.yml
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

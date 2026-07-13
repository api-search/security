---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: milano.it
  spf: false
hosts:
- cert_expires: Feb 13 14:29:50 2027 GMT
  host: dati.comune.milano.it
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dati Comune Milano It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City of Milan Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: City of Milan Open Data
provider_slug: dati-comune-milano-it
slug: dati-comune-milano-it-domain-security
source_filename: dati-comune-milano-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.comune.milano.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 14:29:50 2027 GMT\n  hsts: null\ndomains:\n- domain: milano.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-comune-milano-it/refs/heads/main/security/dati-comune-milano-it-domain-security.yml
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

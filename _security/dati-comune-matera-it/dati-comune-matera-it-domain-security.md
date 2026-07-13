---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: matera.it
  spf: false
hosts:
- cert_expires: Sep 23 15:08:05 2026 GMT
  host: dati.comune.matera.it
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dati Comune Matera It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portale Dati aperti del Comune di Matera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Portale Dati aperti del Comune di Matera
provider_slug: dati-comune-matera-it
slug: dati-comune-matera-it-domain-security
source_filename: dati-comune-matera-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.comune.matera.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 15:08:05 2026 GMT\n  hsts: false\ndomains:\n- domain: matera.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-comune-matera-it/refs/heads/main/security/dati-comune-matera-it-domain-security.yml
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

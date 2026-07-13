---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: roma.it
  spf: false
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: dati.comune.roma.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dati Comune Roma It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rome Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rome Open Data
provider_slug: dati-comune-roma-it
slug: dati-comune-roma-it-domain-security
source_filename: dati-comune-roma-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.comune.roma.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: roma.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-comune-roma-it/refs/heads/main/security/dati-comune-roma-it-domain-security.yml
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

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: torino.it
  spf: false
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: aperto.comune.torino.it
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aperto Comune Torino It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turin Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Turin Open Data
provider_slug: aperto-comune-torino-it
slug: aperto-comune-torino-it-domain-security
source_filename: aperto-comune-torino-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aperto.comune.torino.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: torino.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aperto-comune-torino-it/refs/heads/main/security/aperto-comune-torino-it-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Italy
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dati.gov.it
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.dati.gov.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dati Gov It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dati.gov.it, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: dati.gov.it
provider_slug: dati-gov-it
slug: dati-gov-it-domain-security
source_filename: dati-gov-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dati.gov.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dati.gov.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-gov-it/refs/heads/main/security/dati-gov-it-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Italy
---

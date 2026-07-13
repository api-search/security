---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: open.nrw
  spf: false
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: open.nrw
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Nrw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for open NRW, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: open NRW
provider_slug: open-nrw
slug: open-nrw-domain-security
source_filename: open-nrw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.nrw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: open.nrw\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-nrw/refs/heads/main/security/open-nrw-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Germany
---

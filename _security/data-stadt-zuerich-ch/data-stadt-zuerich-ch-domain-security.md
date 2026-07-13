---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stadt-zuerich.ch
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: data.stadt-zuerich.ch
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Stadt Zuerich Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zurich Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zurich Open Data
provider_slug: data-stadt-zuerich-ch
slug: data-stadt-zuerich-ch-domain-security
source_filename: data-stadt-zuerich-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.stadt-zuerich.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: stadt-zuerich.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-stadt-zuerich-ch/refs/heads/main/security/data-stadt-zuerich-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Switzerland
---

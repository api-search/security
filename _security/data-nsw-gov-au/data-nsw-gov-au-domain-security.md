---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nsw.gov.au
  spf: true
hosts:
- cert_expires: Sep 24 01:44:08 2026 GMT
  host: data.nsw.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Nsw Gov Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NSW Government Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NSW Government Open Data
provider_slug: data-nsw-gov-au
slug: data-nsw-gov-au-domain-security
source_filename: data-nsw-gov-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.nsw.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 01:44:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nsw.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-nsw-gov-au/refs/heads/main/security/data-nsw-gov-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- Australia
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ontario.ca
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: data.ontario.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Ontario Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ontario Data Catalogue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ontario Data Catalogue
provider_slug: data-ontario-ca
slug: data-ontario-ca-domain-security
source_filename: data-ontario-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.ontario.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ontario.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-ontario-ca/refs/heads/main/security/data-ontario-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Provincial Government
- Canada
---

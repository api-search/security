---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kildarecoco.ie
  spf: true
hosts:
- cert_expires: Sep 12 18:08:40 2026 GMT
  host: data.kildarecoco.ie
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Kildarecoco Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kildare County Council Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kildare County Council Open Data
provider_slug: data-kildarecoco-ie
slug: data-kildarecoco-ie-domain-security
source_filename: data-kildarecoco-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.kildarecoco.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:08:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kildarecoco.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-kildarecoco-ie/refs/heads/main/security/data-kildarecoco-ie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- County Government
- Ireland
---

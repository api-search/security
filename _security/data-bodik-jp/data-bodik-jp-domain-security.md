---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bodik.jp
  spf: true
hosts:
- cert_expires: Oct 27 03:08:00 2026 GMT
  host: data.bodik.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data Bodik Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BODIK ODCS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BODIK ODCS
provider_slug: data-bodik-jp
slug: data-bodik-jp-domain-security
source_filename: data-bodik-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.bodik.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 27 03:08:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bodik.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-bodik-jp/refs/heads/main/security/data-bodik-jp-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Organization
- Japan
---

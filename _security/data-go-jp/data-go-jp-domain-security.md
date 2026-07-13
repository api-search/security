---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: go.jp
  spf: false
hosts:
- cert_expires: Nov 12 14:59:59 2026 GMT
  host: www.data.go.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Go Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DATA GO JP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DATA GO JP
provider_slug: data-go-jp
slug: data-go-jp-domain-security
source_filename: data-go-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.data.go.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 14:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: go.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-go-jp/refs/heads/main/security/data-go-jp-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Japan
---

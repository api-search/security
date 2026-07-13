---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: go.jp
  spf: false
hosts:
- cert_expires: Apr  5 09:22:36 2027 GMT
  host: data.e-gov.go.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data E Gov Go Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for e-Gov Data Catalog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: e-Gov Data Catalog
provider_slug: data-e-gov-go-jp
slug: data-e-gov-go-jp-domain-security
source_filename: data-e-gov-go-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.e-gov.go.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 09:22:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: go.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-e-gov-go-jp/refs/heads/main/security/data-e-gov-go-jp-domain-security.yml
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

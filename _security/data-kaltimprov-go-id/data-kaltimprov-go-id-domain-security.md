---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: go.id
  spf: false
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: data.kaltimprov.go.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Kaltimprov Go Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Satu Data Kalimantan Timur, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Satu Data Kalimantan Timur
provider_slug: data-kaltimprov-go-id
slug: data-kaltimprov-go-id-domain-security
source_filename: data-kaltimprov-go-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.kaltimprov.go.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: go.id\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-kaltimprov-go-id/refs/heads/main/security/data-kaltimprov-go-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Provincial Government
- Indonesia
---

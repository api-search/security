---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: go.id
  spf: false
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: data.acehprov.go.id
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data Acehprov Go Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Satu Data Aceh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Satu Data Aceh
provider_slug: data-acehprov-go-id
slug: data-acehprov-go-id-domain-security
source_filename: data-acehprov-go-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.acehprov.go.id\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: go.id\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-acehprov-go-id/refs/heads/main/security/data-acehprov-go-id-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Provincial Government
- Indonesia
---

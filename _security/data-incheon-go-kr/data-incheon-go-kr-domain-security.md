---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: go.kr
  spf: false
hosts:
- cert_expires: Dec  9 05:17:13 2026 GMT
  host: data.incheon.go.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Incheon Go Kr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incheon Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Incheon Open Data
provider_slug: data-incheon-go-kr
slug: data-incheon-go-kr-domain-security
source_filename: data-incheon-go-kr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.incheon.go.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 05:17:13 2026 GMT\n  hsts: false\ndomains:\n- domain: go.kr\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-incheon-go-kr/refs/heads/main/security/data-incheon-go-kr-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Open Data
- DKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- South Korea
---

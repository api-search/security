---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: kommune.no
  spf: false
hosts:
- cert_expires: Apr 20 23:59:59 2027 GMT
  host: www.oslo.kommune.no
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oslo kommune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oslo kommune, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Oslo kommune
provider_slug: oslo-kommune-no
slug: oslo-kommune-no-domain-security
source_filename: oslo-kommune-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oslo.kommune.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kommune.no\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/oslo-kommune-no/security/oslo-kommune-no-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Government
- Municipality
- Norway
- Open Data
- Statistics
- PxWeb
- Public Sector
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lexvector.eu
  spf: true
hosts:
- cert_expires: Jan 29 01:30:37 2027 GMT
  host: lexvector.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LexVector Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LexVector, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: LexVector
provider_slug: lexvector-eu
slug: lexvector-eu-domain-security
source_filename: lexvector-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lexvector.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 01:30:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lexvector.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lexvector-eu/security/lexvector-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Legal Tech
- Search
- Slovakia
---

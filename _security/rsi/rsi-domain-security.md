---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rsi.com
  spf: true
hosts:
- cert_expires: Dec 19 04:26:09 2026 GMT
  host: rsi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rsi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relational Semantics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Relational Semantics
provider_slug: rsi
slug: rsi-domain-security
source_filename: rsi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rsi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 04:26:09 2026 GMT\n  hsts: false\ndomains:\n- domain: rsi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/rsi/security/rsi-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data-Modeling
- Analytics
- APIs
- Enterprise
- Semantic-Data
---

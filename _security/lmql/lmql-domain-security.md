---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lmql.ai
  spf: true
hosts:
- cert_expires: Nov 26 16:47:51 2026 GMT
  host: lmql.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lmql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LMQL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LMQL
provider_slug: lmql
slug: lmql-domain-security
source_filename: lmql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lmql.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 16:47:51 2026 GMT\n  hsts: false\ndomains:\n- domain: lmql.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lmql/security/lmql-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Query Language
- LLM
- Open Source
---

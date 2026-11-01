---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: properfinance.io
  spf: false
hosts:
- cert_expires: Jan  4 06:39:06 2027 GMT
  host: www.properfinance.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Properfinance Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Proper
provider_slug: properfinance-io
slug: properfinance-io-domain-security
source_filename: properfinance-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.properfinance.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 06:39:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: properfinance.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/properfinance-io/security/properfinance-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Reconciliation
- API
- Platform
- SaaS
---

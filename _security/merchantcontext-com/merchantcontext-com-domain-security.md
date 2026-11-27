---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: merchantcontext.com
  spf: true
hosts:
- cert_expires: Feb  3 00:31:56 2027 GMT
  host: merchantcontext.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Merchant Context Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merchant Context, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Merchant Context
provider_slug: merchantcontext-com
slug: merchantcontext-com-domain-security
source_filename: merchantcontext-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merchantcontext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 00:31:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: merchantcontext.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/merchantcontext-com/security/merchantcontext-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Home Services
- Artificial Intelligence
- Search Optimization
- Website Development
- Data Verification
---

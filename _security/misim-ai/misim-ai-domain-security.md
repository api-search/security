---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: misim.ai
  spf: false
hosts:
- cert_expires: Dec 25 22:10:01 2026 GMT
  host: misim.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MISIM.AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MISIM.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MISIM.AI
provider_slug: misim-ai
slug: misim-ai-domain-security
source_filename: misim-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: misim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 22:10:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: misim.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/misim-ai/security/misim-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Tax
- Artificial Intelligence
- Israel
- Accounting
---

---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: khanex.ai
  spf: true
hosts:
- cert_expires: Jan 11 11:08:00 2027 GMT
  host: khanex.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Khanex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Khanex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Khanex
provider_slug: khanex-ai
slug: khanex-ai-domain-security
source_filename: khanex-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: khanex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 11:08:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: khanex.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/khanex-ai/security/khanex-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Consulting
- Development
- Automation
- Product
- Services
---

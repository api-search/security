---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: northlit.ai
  spf: false
hosts:
- cert_expires: Jan  7 22:54:56 2027 GMT
  host: northlit.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Northlit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northlit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Northlit
provider_slug: northlit-ai
slug: northlit-ai-domain-security
source_filename: northlit-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: northlit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 22:54:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: northlit.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/northlit-ai/security/northlit-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Design
- Creative
- Collaboration
---

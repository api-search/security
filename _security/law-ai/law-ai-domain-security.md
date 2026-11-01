---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: law.ai
  spf: true
hosts:
- cert_expires: Jan 19 18:17:18 2027 GMT
  host: law.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Law Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for law-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: law-ai
provider_slug: law-ai
slug: law-ai-domain-security
source_filename: law-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: law.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 18:17:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: law.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/law-ai/security/law-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LegalTech
- AI
- Law
- Directory
- Marketplace
---

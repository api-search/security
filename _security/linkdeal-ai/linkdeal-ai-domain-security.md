---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linkdeal.ai
  spf: true
hosts:
- cert_expires: Jan 21 21:17:28 2027 GMT
  host: linkdeal.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LinkDeal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkDeal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LinkDeal
provider_slug: linkdeal-ai
slug: linkdeal-ai-domain-security
source_filename: linkdeal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkdeal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 21:17:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: linkdeal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/linkdeal-ai/security/linkdeal-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Sales
- Lead Generation
- LinkedIn
- Software-as-a-Service
---

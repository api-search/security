---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kobold.ai
  spf: true
hosts:
- cert_expires: Apr 18 23:59:59 2027 GMT
  host: kobold.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kobold Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KoBold Metals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: KoBold Metals
provider_slug: kobold-ai
slug: kobold-ai-domain-security
source_filename: kobold-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kobold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: kobold.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kobold-ai/security/kobold-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- SaaS
- Marketing
- DataQuality
---

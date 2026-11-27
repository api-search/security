---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hypd.ai
  spf: true
hosts:
- cert_expires: Jan  8 17:43:19 2027 GMT
  host: hypd.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HYPD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HYPD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HYPD
provider_slug: hypd-ai
slug: hypd-ai-domain-security
source_filename: hypd-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hypd.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 17:43:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hypd.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hypd-ai/security/hypd-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Marketing
- Advertising
- GDPR
---

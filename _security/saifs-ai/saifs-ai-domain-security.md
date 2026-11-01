---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: saifs.ai
  spf: true
hosts:
- cert_expires: Dec 11 20:53:06 2026 GMT
  host: saifs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saifs Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for saifs-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: saifs-ai
provider_slug: saifs-ai
slug: saifs-ai-domain-security
source_filename: saifs-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saifs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 20:53:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: saifs.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/saifs-ai/security/saifs-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Content Creation
- Video Generation
- Image Generation
- Audio Generation
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fibr.ai
  spf: true
hosts:
- cert_expires: Aug 20 12:16:08 2026 GMT
  host: fibr.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fibr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fibr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fibr
provider_slug: fibr
slug: fibr-domain-security
source_filename: fibr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fibr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 12:16:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fibr.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fibr/refs/heads/main/security/fibr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Conversion Rate Optimization
- Personalization
- Landing Pages
- A/B Testing
- Experimentation
- Marketing
- Artificial Intelligence
- Agentic Web
- Web Experience
---

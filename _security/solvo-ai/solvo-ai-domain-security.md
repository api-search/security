---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solvo.ai
  spf: true
hosts:
- cert_expires: Sep 24 12:00:54 2026 GMT
  host: www.solvo.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solvo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solvo.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Solvo.ai
provider_slug: solvo-ai
slug: solvo-ai-domain-security
source_filename: solvo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solvo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:00:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: solvo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solvo-ai/refs/heads/main/security/solvo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Container Shipping
- Revenue Management
- Dynamic Pricing
- Freight
- Artificial Intelligence
- Supply Chain
---

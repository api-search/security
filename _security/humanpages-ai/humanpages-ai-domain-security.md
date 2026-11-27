---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humanpages.ai
  spf: true
hosts:
- cert_expires: Dec 31 10:05:42 2026 GMT
  host: humanpages.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Human Pages Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Human Pages, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Human Pages
provider_slug: humanpages-ai
slug: humanpages-ai-domain-security
source_filename: humanpages-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanpages.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 10:05:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humanpages.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/humanpages-ai/security/humanpages-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- Artificial Intelligence
- Human Workforce
- Gig Economy
- Zero Fees
---

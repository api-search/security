---
api_specs:
- filename: memoket-ai-openapi-generated.yml
  format: yaml
  label: Memoket API
  slug: memoket-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memoket-ai/openapi/_ae-authored/memoket-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memoket.ai
  spf: true
hosts:
- cert_expires: Jan  6 16:00:05 2027 GMT
  host: memoket.ai
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memoket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memoket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Memoket
provider_slug: memoket-ai
slug: memoket-ai-domain-security
source_filename: memoket-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memoket.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 16:00:05 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: memoket.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/memoket-ai/security/memoket-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Wearables
- Productivity
- Privacy
---

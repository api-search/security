---
api_specs:
- filename: bunny-com-openapi-generated.yml
  format: yaml
  label: Bunny API
  slug: bunny-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bunny-com/openapi/_ae-authored/bunny-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bunny.com
  spf: true
hosts:
- cert_expires: Dec 13 15:23:51 2026 GMT
  host: bunny.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bunny Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bunny, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bunny
provider_slug: bunny-com
slug: bunny-com-domain-security
source_filename: bunny-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bunny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 15:23:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bunny.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bunny-com/security/bunny-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- CPQ
- Revenue Recognition
- SaaS Analytics
- Revenue Operations
- Stripe Integration
- AI Agents
---

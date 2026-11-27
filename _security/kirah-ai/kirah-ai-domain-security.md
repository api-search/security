---
api_specs:
- filename: kirah-ai-openapi-generated.yml
  format: yaml
  label: Kirah API
  slug: kirah-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kirah-ai/openapi/_ae-authored/kirah-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kirah.ai
  spf: false
hosts:
- cert_expires: Jan  4 00:26:12 2027 GMT
  host: kirah.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kirah Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kirah, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Kirah
provider_slug: kirah-ai
slug: kirah-ai-domain-security
source_filename: kirah-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kirah.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 00:26:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kirah.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kirah-ai/security/kirah-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wellness
- Artificial Intelligence
- Booking
- Healthcare
---

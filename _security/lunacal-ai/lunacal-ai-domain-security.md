---
api_specs:
- filename: lunacal-ai-openapi-generated.yml
  format: yaml
  label: Lunacal API
  slug: lunacal-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lunacal-ai/openapi/_ae-authored/lunacal-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunacal.ai
  spf: true
hosts:
- cert_expires: Jan 14 14:51:32 2027 GMT
  host: lunacal.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lunacal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunacal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lunacal
provider_slug: lunacal-ai
slug: lunacal-ai-domain-security
source_filename: lunacal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lunacal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 14:51:32 2027 GMT\n  hsts: false\ndomains:\n- domain: lunacal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lunacal-ai/security/lunacal-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Scheduling
- Appointment
- Artificial Intelligence
- Software-as-a-Service
- Business
---

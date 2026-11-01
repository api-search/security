---
api_specs:
- filename: phoebe-ai-openapi-generated.yml
  format: yaml
  label: Phoebe API
  slug: phoebe-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phoebe-ai/openapi/_ae-authored/phoebe-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: phoebe.ai
  spf: true
hosts:
- cert_expires: Dec 31 08:05:59 2026 GMT
  host: phoebe.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Phoebe Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phoebe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Phoebe
provider_slug: phoebe-ai
slug: phoebe-ai-domain-security
source_filename: phoebe-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phoebe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 08:05:59 2026 GMT\n  hsts: false\ndomains:\n- domain: phoebe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/phoebe-ai/security/phoebe-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Machine-Learning
- Platform
- Ethics
- Enterprise
---

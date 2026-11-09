---
api_specs:
- filename: audo-ai-api-openapi.json
  format: json
  label: Audo API API
  slug: audo-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audo-ai/openapi/_original/audo-ai-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audo.ai
  spf: true
hosts:
- cert_expires: Dec 31 04:01:00 2026 GMT
  host: audo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Audo
provider_slug: audo-ai
slug: audo-ai-domain-security
source_filename: audo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 04:01:00 2026 GMT\n  hsts: false\ndomains:\n- domain: audo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/audo-ai/security/audo-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Audio
- Video
- Tools
---

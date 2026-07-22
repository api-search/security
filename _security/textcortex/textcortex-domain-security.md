---
api_specs:
- filename: textcortex-openapi.json
  format: json
  label: TextCortex API
  slug: textcortex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textcortex/refs/heads/main/openapi/textcortex-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: textcortex.com
  spf: true
hosts:
- cert_expires: Sep 14 23:03:28 2026 GMT
  host: api.textcortex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Textcortex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Textcortex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Textcortex
provider_slug: textcortex
slug: textcortex-domain-security
source_filename: textcortex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.textcortex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:03:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: textcortex.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textcortex/refs/heads/main/security/textcortex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Text Generation
- Large Language Models
- Chat Completions
- OpenAI-Compatible
- Content Generation
- Developer Tools
---

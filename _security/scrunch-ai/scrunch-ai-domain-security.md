---
api_specs:
- filename: scrunch-ai-data-api-openapi.yml
  format: yaml
  label: Scrunch Data API
  slug: scrunch-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scrunchai.com
  spf: true
hosts:
- cert_expires: Oct 11 07:34:26 2026 GMT
  host: scrunchai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 11:44:10 2026 GMT
  host: api.scrunchai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrunch Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scrunch AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scrunch AI
provider_slug: scrunch-ai
slug: scrunch-ai-domain-security
source_filename: scrunch-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scrunchai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:34:26 2026 GMT\n  hsts: false\n- host: api.scrunchai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:44:10 2026 GMT\n  hsts: null\ndomains:\n- domain: scrunchai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/security/scrunch-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- AI Search
- Answer Engine Optimization
- Generative Engine Optimization
- Brand Visibility
- Analytics
- SEO
- Agent Experience
- MCP
---

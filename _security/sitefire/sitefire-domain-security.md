---
api_specs:
- filename: sitefire-book-demo-openapi.yml
  format: yaml
  label: Sitefire Book-a-Demo API
  slug: sitefire-book-a-demo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitefire/refs/heads/main/openapi/sitefire-book-demo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sitefire.ai
  spf: true
hosts:
- cert_expires: Oct 14 22:36:38 2026 GMT
  host: sitefire.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sitefire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sitefire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sitefire
provider_slug: sitefire
slug: sitefire-domain-security
source_filename: sitefire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sitefire.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:36:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sitefire.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitefire/refs/heads/main/security/sitefire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Generative Engine Optimization
- AI Visibility
- Marketing
- SEO
- Analytics
- Artificial Intelligence
- Content Generation
- MCP
- Agent
---

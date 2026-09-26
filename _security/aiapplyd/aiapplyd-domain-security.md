---
api_specs:
- filename: aiapplyd-openapi.yml
  format: yaml
  label: AI Applyd API
  slug: ai-applyd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aiapplyd/refs/heads/main/openapi/aiapplyd-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aiapplyd.com
  spf: true
hosts:
- cert_expires: Dec  8 13:43:48 2026 GMT
  host: aiapplyd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 12:56:19 2026 GMT
  host: api.aiapplyd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 11:39:48 2026 GMT
  host: mcp.aiapplyd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aiapplyd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Applyd, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AI Applyd
provider_slug: aiapplyd
slug: aiapplyd-domain-security
source_filename: aiapplyd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiapplyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 13:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aiapplyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 12:56:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.aiapplyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:39:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aiapplyd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiapplyd/refs/heads/main/security/aiapplyd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Job Search
- Recruiting
- Resume
- Applicant Tracking Systems
- Careers
- Artificial Intelligence
- MCP
- Automation
---

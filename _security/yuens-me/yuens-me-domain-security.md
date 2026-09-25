---
api_specs:
- filename: yuens-me-openapi.yml
  format: yaml
  label: Resume Agent API
  slug: resume-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuens-me/refs/heads/main/openapi/yuens-me-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yuens.me
  spf: true
hosts:
- cert_expires: Dec 13 18:49:20 2026 GMT
  host: yuens.me
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 22:10:15 2026 GMT
  host: agent.yuens.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Yuens Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunny Yuen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sunny Yuen
provider_slug: yuens-me
slug: yuens-me-domain-security
source_filename: yuens-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yuens.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 18:49:20 2026 GMT\n  hsts: null\n- host: agent.yuens.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 22:10:15 2026 GMT\n  hsts: false\ndomains:\n- domain: yuens.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuens-me/refs/heads/main/security/yuens-me-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI Agents
- A2A
- MCP
- Resume
- Hiring
- Recruiting
- Professional Profile
- Job Matching
- Open Source
---

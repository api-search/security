---
api_specs:
- filename: humanbrowser-cloud-openapi.json
  format: json
  label: Human Browser API
  slug: human-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanbrowser-cloud/refs/heads/main/openapi/humanbrowser-cloud-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: humanbrowser.cloud
  spf: true
hosts:
- cert_expires: Dec  1 18:33:01 2026 GMT
  host: humanbrowser.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 18:33:01 2026 GMT
  host: agent.humanbrowser.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Humanbrowser Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virix Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Virix Labs
provider_slug: humanbrowser-cloud
slug: humanbrowser-cloud-domain-security
source_filename: humanbrowser-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanbrowser.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 18:33:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: agent.humanbrowser.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 18:33:01 2026 GMT\n  hsts: null\ndomains:\n- domain: humanbrowser.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanbrowser-cloud/refs/heads/main/security/humanbrowser-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Browser Automation
- Cloud Browser
- AI Agents
- A2A
- MCP
- Web Scraping
- Residential Proxies
- CAPTCHA Solving
- Human-in-the-Loop
- Computer Use
- Agent-Native
- United Kingdom
---

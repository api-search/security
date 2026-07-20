---
api_specs:
- filename: graphy-agents-openapi.yaml
  format: yaml
  label: Graphy AI Agents API
  slug: graphy-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphy/refs/heads/main/openapi/graphy-agents-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: graphy.app
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: graphy.dev
  spf: true
hosts:
- cert_expires: Sep 10 14:40:46 2026 GMT
  host: graphy.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 01:21:53 2026 GMT
  host: agents.graphy.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graphy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graphy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Graphy
provider_slug: graphy
slug: graphy-domain-security
source_filename: graphy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graphy.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:40:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agents.graphy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 01:21:53 2026 GMT\n  hsts: null\ndomains:\n- domain: graphy.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: graphy.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphy/refs/heads/main/security/graphy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Visualization
- Charts
- Charting
- Analytics
- Artificial Intelligence
- Data Storytelling
- Developer Tools
- SDK
- Agents
---

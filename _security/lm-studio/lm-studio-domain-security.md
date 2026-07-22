---
api_specs:
- filename: lm-studio-server-openapi.yml
  format: yaml
  label: LM Studio Local Server API
  slug: lm-studio-local-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lm-studio/refs/heads/main/openapi/lm-studio-server-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lmstudio.ai
  spf: true
hosts:
- cert_expires: Oct  4 12:45:40 2026 GMT
  host: lmstudio.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lm Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LM Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: LM Studio
provider_slug: lm-studio
slug: lm-studio-domain-security
source_filename: lm-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lmstudio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:45:40 2026 GMT\n  hsts: false\ndomains:\n- domain: lmstudio.ai\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lm-studio/refs/heads/main/security/lm-studio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Ai
- Local LLM
- Machine Learning
- Inference
- Developer Tools
- LLM
- MCP
- SDK
- Desktop Application
---

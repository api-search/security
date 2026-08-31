---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kleio.ai
  spf: true
hosts:
- cert_expires: Nov  4 04:54:19 2026 GMT
  host: www.kleio.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 04:54:19 2026 GMT
  host: api.kleio.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: HSTS corrected by hand after the automated probe recorded null. api.kleio.ai answers every undefined path with a JSON 404 from its Google Cloud API Gateway, which the probe treated as no header; a direct HEAD returns two Strict-Transport-Security headers — "max-age=15552000; includeSubDomains; preload" (Cloudflare edge) and "max-age=31536000; includeSubDomains" (origin). The longer max-age is recorded.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kleio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kleio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kleio
provider_slug: kleio
slug: kleio-domain-security
source_filename: kleio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kleio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 04:54:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kleio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 04:54:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: 'HSTS corrected by hand after the automated probe recorded null. api.kleio.ai answers every\n    undefined path with a JSON 404 from its Google Cloud API Gateway, which the probe treated as no\n    header; a direct HEAD returns two Strict-Transport-Security headers — \"max-age=15552000;\n    includeSubDomains; preload\" (Cloudflare edge) and \"max-age=31536000; includeSubDomains\" (origin).\n    The longer max-age is recorded.'\ndomains:\n- domain: kleio.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kleio/refs/heads/main/security/kleio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai Data
- Agentic Commerce
- AI Agents
- Enterprise Sales
- Conversational AI
- Knowledge Engine
- MCP
- Agent To Agent
- Retail
- Travel
- Real-Estate
- Automotive
- France
---

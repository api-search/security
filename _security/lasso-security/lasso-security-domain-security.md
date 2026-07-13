---
api_specs:
- filename: lasso-security-openapi.yml
  format: yaml
  label: Lasso Classify / Threat Detection API
  slug: classify-threat-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/openapi/lasso-security-openapi.yml
- filename: lasso-security-openapi.yml
  format: yaml
  label: Lasso LLM Gateway (Deputy)
  slug: llm-gateway-deputy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/openapi/lasso-security-openapi.yml
- filename: lasso-security-openapi.yml
  format: yaml
  label: Lasso MCP Gateway
  slug: mcp-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/openapi/lasso-security-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:devops@lasso.security"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lasso.security
  spf: true
hosts:
- cert_expires: Aug 22 18:16:44 2026 GMT
  host: www.lasso.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: server.lasso.security
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lasso Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lasso Security, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lasso Security
provider_slug: lasso-security
slug: lasso-security-domain-security
source_filename: lasso-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lasso.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:16:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: server.lasso.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lasso.security\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:devops@lasso.security\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/security/lasso-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- GenAI Security
- Prompt Injection
- Guardrails
- MCP
---

---
api_specs:
- filename: leena-ai-analytics-api-openapi.yml
  format: yaml
  label: Leena AI Analytics API
  slug: leena-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-analytics-api-openapi.yml
- filename: leena-ai-aop-api-openapi.yml
  format: yaml
  label: Leena AI AOP API
  slug: leena-ai-aop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-aop-api-openapi.yml
- filename: leena-ai-audit-logs-api-openapi.yml
  format: yaml
  label: Leena AI Audit Logs API
  slug: leena-ai-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-audit-logs-api-openapi.yml
- filename: leena-ai-authentication-api-openapi.yml
  format: yaml
  label: Leena AI Authentication API
  slug: leena-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-authentication-api-openapi.yml
- filename: leena-ai-knowledge-articles-api-openapi.yml
  format: yaml
  label: Leena AI Knowledge Articles API
  slug: leena-ai-knowledge-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-knowledge-articles-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leena.ai
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: leena.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 15:58:51 2026 GMT
  host: docs.leena.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: us-east-1-aic.leena.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leena Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leena AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Leena AI
provider_slug: leena-ai
slug: leena-ai-domain-security
source_filename: leena-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leena.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.leena.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 15:58:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us-east-1-aic.leena.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: leena.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/security/leena-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Agentic AI
- Artificial Intelligence
- Enterprise Software
- Human Resources
- IT Service Management
- Employee Experience
- Workflow Automation
- Conversational AI
- Model Context Protocol
- Knowledge Management
---

---
api_specs:
- filename: celonis-knowledge-model-openapi.yaml
  format: yaml
  label: Celonis Knowledge Model API
  slug: celonis-knowledge-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-knowledge-model-openapi.yaml
- filename: celonis-agents-ai-openapi.yaml
  format: yaml
  label: Celonis AI Agent API
  slug: celonis-ai-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-agents-ai-openapi.yaml
- filename: celonis-subscription-openapi.yaml
  format: yaml
  label: Celonis Event Subscription API
  slug: celonis-event-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-subscription-openapi.yaml
- filename: celonis-mlwb-openapi.yaml
  format: yaml
  label: Celonis Machine Learning Workbench API
  slug: celonis-machine-learning-workbench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-mlwb-openapi.yaml
- filename: celonis-team-openapi.yaml
  format: yaml
  label: Celonis Team API
  slug: celonis-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-team-openapi.yaml
- filename: celonis-permissions-openapi.yaml
  format: yaml
  label: Celonis Permissions API
  slug: celonis-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-permissions-openapi.yaml
- filename: celonis-mcp-tool-calling-openapi.yaml
  format: yaml
  label: Celonis Agent Tools (MCP) Tool Calling API
  slug: celonis-agent-tools-mcp-tool-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-mcp-tool-calling-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:internalsupport@celonis.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "certainly.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: celonis.com
  spf: true
hosts:
- cert_expires: Oct 16 09:39:47 2026 GMT
  host: www.celonis.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Celonis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celonis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Celonis
provider_slug: celonis
slug: celonis-domain-security
source_filename: celonis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.celonis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 09:39:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: celonis.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:internalsupport@celonis.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/security/celonis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automation
- Process Mining
- Process Intelligence
- Data
- Analytics
- Machine Learning
- AI Agents
- Enterprise
---

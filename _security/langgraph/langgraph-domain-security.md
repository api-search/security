---
api_specs:
- filename: langgraph-agent-connections-v2-api-openapi.yml
  format: yaml
  label: LangGraph Agent Connections (v2) API
  slug: langgraph-agent-connections-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-agent-connections-v2-api-openapi.yml
- filename: langgraph-auth-service-v2-api-openapi.yml
  format: yaml
  label: LangGraph Auth Service (v2) API
  slug: langgraph-auth-service-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-auth-service-v2-api-openapi.yml
- filename: langgraph-deployments-v2-api-openapi.yml
  format: yaml
  label: LangGraph Deployments (v2) API
  slug: langgraph-deployments-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-deployments-v2-api-openapi.yml
- filename: langgraph-integrations-v1-api-openapi.yml
  format: yaml
  label: LangGraph Integrations (v1) API
  slug: langgraph-integrations-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-integrations-v1-api-openapi.yml
- filename: langgraph-listeners-v2-api-openapi.yml
  format: yaml
  label: LangGraph Listeners (v2) API
  slug: langgraph-listeners-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-listeners-v2-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: langchain.com
  spf: true
hosts:
- cert_expires: Oct  1 02:45:45 2026 GMT
  host: www.langchain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 16:49:13 2026 GMT
  host: docs.langchain.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:21:48 2026 GMT
  host: api.host.langchain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Langgraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LangGraph, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LangGraph
provider_slug: langgraph
slug: langgraph-domain-security
source_filename: langgraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.langchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:45:45 2026 GMT\n  hsts: false\n- host: docs.langchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:49:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.host.langchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:21:48 2026 GMT\n  hsts: null\ndomains:\n- domain: langchain.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/security/langgraph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agents
- Artificial Intelligence
- Large Language Models
- Workflows
- Orchestration
---

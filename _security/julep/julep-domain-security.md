---
api_specs:
- filename: julep-openapi-original.yml
  format: yaml
  label: Julep API
  slug: julep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: julep.ai
  spf: true
hosts:
- cert_expires: Aug 25 08:13:40 2026 GMT
  host: docs.julep.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 05:37:10 2026 GMT
  host: api.julep.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Julep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Julep, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Julep
provider_slug: julep
slug: julep-domain-security
source_filename: julep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.julep.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:13:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.julep.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:37:10 2026 GMT\n  hsts: false\ndomains:\n- domain: julep.ai\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/security/julep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI Agents
- LLM
- Agents
- Workflows
- RAG
- Memory
- Orchestration
- Developer Tools
- Open Source
---

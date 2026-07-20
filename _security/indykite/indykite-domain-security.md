---
api_specs:
- filename: indykite-rest-openapi.yml
  format: yaml
  label: IndyKite REST API
  slug: indykite-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indykite/refs/heads/main/openapi/indykite-rest-openapi.yml
- filename: indykite-config-openapi.yml
  format: yaml
  label: IndyKite Config REST API
  slug: indykite-config-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indykite/refs/heads/main/openapi/indykite-config-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: indykite.com
  spf: true
hosts:
- cert_expires: Oct  2 07:02:31 2026 GMT
  host: eu.api.indykite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 07:07:07 2026 GMT
  host: us.api.indykite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indykite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indykite, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Indykite
provider_slug: indykite
slug: indykite-domain-security
source_filename: indykite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eu.api.indykite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:02:31 2026 GMT\n  hsts: null\n- host: us.api.indykite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:07:07 2026 GMT\n  hsts: null\ndomains:\n- domain: indykite.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indykite/refs/heads/main/security/indykite-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Identity
- Authorization
- Access Control
- Knowledge Graph
- Agentic AI
- MCP
- Security
- AuthZEN
---

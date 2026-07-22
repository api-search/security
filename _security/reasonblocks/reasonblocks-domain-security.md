---
api_specs:
- filename: reasonblocks-openapi-original.json
  format: json
  label: ReasonBlocks REST API
  slug: reasonblocks-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/openapi/reasonblocks-openapi-original.json
description: ''
domains:
- caa:
  - reasonblocks-website.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: reasonblocks.com
  spf: false
hosts:
- cert_expires: Sep 26 05:58:45 2026 GMT
  host: reasonblocks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 10:44:46 2026 GMT
  host: docs.reasonblocks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 17:13:23 2026 GMT
  host: rb-api.reasonblocks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reasonblocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReasonBlocks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: ReasonBlocks
provider_slug: reasonblocks
slug: reasonblocks-domain-security
source_filename: reasonblocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reasonblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:58:45 2026 GMT\n  hsts: false\n- host: docs.reasonblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:44:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rb-api.reasonblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:13:23 2026 GMT\n  hsts: null\ndomains:\n- domain: reasonblocks.com\n  dnssec: true\n  caa:\n  - reasonblocks-website.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reasonblocks/refs/heads/main/security/reasonblocks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI Agents
- Agent Observability
- LLM
- Developer Tools
- Token Optimization
- Agent Steering
- Machine Learning
- Artificial Intelligence
- SDK
---

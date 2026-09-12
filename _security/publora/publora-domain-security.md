---
api_specs:
- filename: publora-openapi-original.json
  format: json
  label: Publora API
  slug: publora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publora/refs/heads/main/openapi/publora-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: publora.com
  spf: true
hosts:
- cert_expires: Oct 22 13:42:02 2026 GMT
  host: docs.publora.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 13:42:02 2026 GMT
  host: api.publora.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Publora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Publora, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Publora
provider_slug: publora
slug: publora-domain-security
source_filename: publora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.publora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 13:42:02 2026 GMT\n  hsts: false\n- host: api.publora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 13:42:02 2026 GMT\n  hsts: null\ndomains:\n- domain: publora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publora/refs/heads/main/security/publora-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Media
- Publishing
- Scheduling
- MCP
- Content
- Social Media Management
- Webhooks
- AI Agents
---

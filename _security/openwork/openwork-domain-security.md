---
api_specs:
- filename: openwork-den-openapi.json
  format: json
  label: OpenWork Den API
  slug: den-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openwork/refs/heads/main/openapi/openwork-den-openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openworklabs.com
  spf: true
hosts:
- cert_expires: Aug 20 12:31:39 2026 GMT
  host: openworklabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 05:14:45 2026 GMT
  host: api.openworklabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openwork, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Openwork
provider_slug: openwork
slug: openwork-domain-security
source_filename: openwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openworklabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 12:31:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.openworklabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:14:45 2026 GMT\n  hsts: false\ndomains:\n- domain: openworklabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openwork/refs/heads/main/security/openwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Open Source
- Desktop
- Agent Runtime
- MCP
- Control Plane
- SSO
- SCIM
- Developer Tools
---

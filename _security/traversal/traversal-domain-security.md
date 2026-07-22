---
api_specs:
- filename: traversal-sessions-openapi.yaml
  format: yaml
  label: Traversal Sessions API
  slug: traversal-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traversal/refs/heads/main/openapi/traversal-sessions-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: traversal.com
  spf: true
hosts:
- cert_expires: Sep 15 17:47:18 2026 GMT
  host: www.traversal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 19:23:38 2026 GMT
  host: api.traversal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Traversal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traversal, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Traversal
provider_slug: traversal
slug: traversal-domain-security
source_filename: traversal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.traversal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.traversal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:23:38 2026 GMT\n  hsts: null\ndomains:\n- domain: traversal.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traversal/refs/heads/main/security/traversal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- AI SRE
- Site Reliability Engineering
- Observability
- Incident Management
- Root Cause Analysis
- DevOps
- MCP
---

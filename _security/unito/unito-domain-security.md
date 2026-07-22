---
api_specs:
- filename: unito-embeds-openapi-original.json
  format: json
  label: Unito Embed API
  slug: unito-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unito/refs/heads/main/openapi/unito-embeds-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unito.io
  spf: true
hosts:
- cert_expires: Sep 26 01:01:47 2026 GMT
  host: unito.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:58:22 2026 GMT
  host: dev.unito.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:58:22 2026 GMT
  host: api.unito.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unito, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unito
provider_slug: unito
slug: unito-domain-security
source_filename: unito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unito.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:01:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.unito.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:58:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unito.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:58:22 2026 GMT\n  hsts: null\ndomains:\n- domain: unito.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unito/refs/heads/main/security/unito-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Integration
- Two-Way Sync
- Workflow Automation
- Project Management
- Collaboration
- Embedded Integrations
- SaaS
---

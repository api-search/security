---
api_specs:
- filename: pipefy-openapi.yml
  format: yaml
  label: Pipefy GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipefy/refs/heads/main/openapi/pipefy-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pipefy.com
  spf: true
hosts:
- cert_expires: Sep 17 16:58:32 2026 GMT
  host: www.pipefy.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:32:42 2026 GMT
  host: developers.pipefy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 00:15:34 2026 GMT
  host: api.pipefy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pipefy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pipefy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pipefy
provider_slug: pipefy
slug: pipefy-domain-security
source_filename: pipefy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pipefy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:58:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.pipefy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:32:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pipefy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:15:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pipefy.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipefy/refs/heads/main/security/pipefy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Workflow Automation
- Business Process Management
- No-Code
- BPM
- GraphQL
- Process Orchestration
---

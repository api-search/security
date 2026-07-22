---
api_specs:
- filename: workflowy-api-openapi.yml
  format: yaml
  label: Workflowy API
  slug: workflowy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workflowy/refs/heads/main/openapi/workflowy-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workflowy.com
  spf: true
hosts:
- cert_expires: Oct  2 00:11:50 2026 GMT
  host: workflowy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workflowy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workflowy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Workflowy
provider_slug: workflowy
slug: workflowy-domain-security
source_filename: workflowy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workflowy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:11:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: workflowy.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workflowy/refs/heads/main/security/workflowy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Notes
- Outliner
- Task Management
- Lists
- Collaboration
- Knowledge Management
- AI Assistant
---

---
api_specs:
- filename: corestack-external-api-openapi-original.json
  format: json
  label: CoreStack External API
  slug: corestack-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corestack/refs/heads/main/openapi/corestack-external-api-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: corestack.io
  spf: true
hosts:
- cert_expires: Sep 18 15:57:15 2026 GMT
  host: www.corestack.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 21:16:13 2026 GMT
  host: docs.corestack.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 13:19:51 2026 GMT
  host: api.corestack.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corestack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreStack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CoreStack
provider_slug: corestack
slug: corestack-domain-security
source_filename: corestack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corestack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 15:57:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.corestack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 21:16:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.corestack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:19:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corestack.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corestack/refs/heads/main/security/corestack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- cloud-governance
- finops
- cloud-cost-management
- cloud-security-posture-management
- compliance
- multi-cloud
- cnapp
- policy-as-code
- cloudops
- mcp
- agent-native
- kubernetes
---

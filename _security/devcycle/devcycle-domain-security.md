---
api_specs:
- filename: devcycle-management-openapi.json
  format: json
  label: DevCycle Management API
  slug: devcycle-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/openapi/devcycle-management-openapi.json
- filename: devcycle-bucketing-openapi.yaml
  format: yaml
  label: DevCycle Bucketing API
  slug: devcycle-bucketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/openapi/devcycle-bucketing-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: devcycle.com
  spf: true
hosts:
- cert_expires: Aug 28 10:26:28 2026 GMT
  host: www.devcycle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 18:16:07 2026 GMT
  host: bucketing-api.devcycle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 01:28:23 2026 GMT
  host: api.devcycle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devcycle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevCycle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DevCycle
provider_slug: devcycle
slug: devcycle-domain-security
source_filename: devcycle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.devcycle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:26:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bucketing-api.devcycle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:16:07 2026 GMT\n  hsts: null\n- host: api.devcycle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:28:23 2026 GMT\n  hsts: null\ndomains:\n- domain: devcycle.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/security/devcycle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise Saas
- Feature Flags
- Feature Management
- Feature Flags as a Service
- Experimentation
- OpenFeature
- Developer Tools
- DevOps
---

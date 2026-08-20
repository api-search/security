---
api_specs:
- filename: showpad-v3-openapi-original.yml
  format: yaml
  label: Showpad Content API
  slug: showpad-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v3-openapi-original.yml
- filename: showpad-v4-openapi-original.yml
  format: yaml
  label: Showpad API v4
  slug: showpad-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v4-openapi-original.yml
- filename: showpad-v3-openapi-original.yml
  format: yaml
  label: Showpad User Management API
  slug: showpad-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v3-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@showpad.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: showpad.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: developer.showpad.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Showpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Showpad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Showpad
provider_slug: showpad
slug: showpad-domain-security
source_filename: showpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.showpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: showpad.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@showpad.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/security/showpad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Enablement
- Sales Coaching
- Content Management
- Buyer Engagement
- Sales Analytics
- Training
- CRM Integration
- Digital Sales Rooms
- MCP
- SCIM
---

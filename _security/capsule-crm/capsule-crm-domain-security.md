---
api_specs:
- filename: capsule-crm-openapi.yml
  format: yaml
  label: Capsule CRM API v2
  slug: v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule-crm/refs/heads/main/openapi/capsule-crm-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-iodef@zestia.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capsulecrm.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: capsulecrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: developer.capsulecrm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.capsulecrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capsule Crm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capsule CRM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capsule CRM
provider_slug: capsule-crm
slug: capsule-crm-domain-security
source_filename: capsule-crm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capsulecrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.capsulecrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.capsulecrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capsulecrm.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa-iodef@zestia.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capsule-crm/refs/heads/main/security/capsule-crm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Sales
- Contacts
- Pipeline Management
- Tasks
- Projects
- SMB
---

---
api_specs:
- filename: acronis-account-management-openapi.yaml
  format: yaml
  label: Acronis Account Management API
  slug: account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-account-management-openapi.yaml
- filename: acronis-agent-management-openapi.yaml
  format: yaml
  label: Acronis Agent Management REST API
  slug: agent-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-agent-management-openapi.yaml
- filename: acronis-task-manager-openapi.yaml
  format: yaml
  label: Acronis Task Manager API
  slug: task-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-task-manager-openapi.yaml
description: ''
domains:
- caa:
  - 0 iodef "mailto:hostmaster@acronis.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acronis.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: developer.acronis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acronis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acronis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Acronis
provider_slug: acronis
slug: acronis-domain-security
source_filename: acronis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.acronis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acronis.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hostmaster@acronis.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/security/acronis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
---

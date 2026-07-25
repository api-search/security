---
api_specs:
- filename: acronis-activities-api-openapi.yml
  format: yaml
  label: Acronis Activities API
  slug: acronis-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-activities-api-openapi.yml
- filename: acronis-agent-updates-api-openapi.yml
  format: yaml
  label: Acronis Agent Updates API
  slug: acronis-agent-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-agent-updates-api-openapi.yml
- filename: acronis-agents-api-openapi.yml
  format: yaml
  label: Acronis Agents API
  slug: acronis-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-agents-api-openapi.yml
- filename: acronis-authentication-api-openapi.yml
  format: yaml
  label: Acronis Authentication API
  slug: acronis-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-authentication-api-openapi.yml
- filename: acronis-clients-api-openapi.yml
  format: yaml
  label: Acronis Clients API
  slug: acronis-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-clients-api-openapi.yml
- filename: acronis-hardware-nodes-api-openapi.yml
  format: yaml
  label: Acronis Hardware Nodes API
  slug: acronis-hardware-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-hardware-nodes-api-openapi.yml
- filename: acronis-licensing-api-openapi.yml
  format: yaml
  label: Acronis Licensing API
  slug: acronis-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-licensing-api-openapi.yml
- filename: acronis-tasks-api-openapi.yml
  format: yaml
  label: Acronis Tasks API
  slug: acronis-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-tasks-api-openapi.yml
- filename: acronis-tenants-api-openapi.yml
  format: yaml
  label: Acronis Tenants API
  slug: acronis-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-tenants-api-openapi.yml
- filename: acronis-usage-api-openapi.yml
  format: yaml
  label: Acronis Usage API
  slug: acronis-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-usage-api-openapi.yml
- filename: acronis-users-api-openapi.yml
  format: yaml
  label: Acronis Users API
  slug: acronis-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/openapi/acronis-users-api-openapi.yml
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

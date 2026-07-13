---
api_specs:
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Customers API
  slug: gorilladesk-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Customer Notes API
  slug: gorilladesk-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Users API
  slug: gorilladesk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Company API
  slug: gorilladesk-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
- filename: gorilladesk-openapi.yml
  format: yaml
  label: GorillaDesk Phone Types API
  slug: gorilladesk-phone-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/openapi/gorilladesk-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gorilladesk.com
  spf: true
hosts:
- cert_expires: Sep 20 23:46:40 2026 GMT
  host: gorilladesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:46:40 2026 GMT
  host: api.gorilladesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gorilladesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GorillaDesk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GorillaDesk
provider_slug: gorilladesk
slug: gorilladesk-domain-security
source_filename: gorilladesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gorilladesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:46:40 2026 GMT\n  hsts: false\n- host: api.gorilladesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:46:40 2026 GMT\n  hsts: null\ndomains:\n- domain: gorilladesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gorilladesk/refs/heads/main/security/gorilladesk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Field Service Management
- Pest Control
- Lawn Care
- Scheduling
- Invoicing
- Customers
- SaaS
---

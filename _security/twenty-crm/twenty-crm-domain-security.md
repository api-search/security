---
api_specs:
- filename: twenty-crm-companies-api-openapi.yml
  format: yaml
  label: Twenty Companies API
  slug: twenty-crm-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-companies-api-openapi.yml
- filename: twenty-crm-metadata-fields-api-openapi.yml
  format: yaml
  label: Twenty Metadata - Fields API
  slug: twenty-crm-metadata-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-metadata-fields-api-openapi.yml
- filename: twenty-crm-metadata-objects-api-openapi.yml
  format: yaml
  label: Twenty Metadata - Objects API
  slug: twenty-crm-metadata-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-metadata-objects-api-openapi.yml
- filename: twenty-crm-notes-api-openapi.yml
  format: yaml
  label: Twenty Notes API
  slug: twenty-crm-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-notes-api-openapi.yml
- filename: twenty-crm-opportunities-api-openapi.yml
  format: yaml
  label: Twenty Opportunities API
  slug: twenty-crm-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-opportunities-api-openapi.yml
- filename: twenty-crm-people-api-openapi.yml
  format: yaml
  label: Twenty People API
  slug: twenty-crm-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-people-api-openapi.yml
- filename: twenty-crm-tasks-api-openapi.yml
  format: yaml
  label: Twenty Tasks API
  slug: twenty-crm-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-tasks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: twenty.com
  spf: true
hosts:
- cert_expires: Sep  6 23:59:45 2026 GMT
  host: twenty.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:20:05 2026 GMT
  host: docs.twenty.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 20:32:08 2026 GMT
  host: api.twenty.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twenty Crm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twenty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Twenty
provider_slug: twenty-crm
slug: twenty-crm-domain-security
source_filename: twenty-crm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: twenty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:59:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.twenty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:20:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.twenty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 20:32:08 2026 GMT\n  hsts: null\ndomains:\n- domain: twenty.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/security/twenty-crm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Open Source
- Sales
- GraphQL
- REST
---

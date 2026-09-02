---
api_specs:
- filename: copper-activities-api-openapi.yml
  format: yaml
  label: Copper Activities API
  slug: copper-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/openapi/copper-activities-api-openapi.yml
- filename: copper-companies-api-openapi.yml
  format: yaml
  label: Copper Companies API
  slug: copper-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/openapi/copper-companies-api-openapi.yml
- filename: copper-leads-api-openapi.yml
  format: yaml
  label: Copper Leads API
  slug: copper-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/openapi/copper-leads-api-openapi.yml
- filename: copper-opportunities-api-openapi.yml
  format: yaml
  label: Copper Opportunities API
  slug: copper-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/openapi/copper-opportunities-api-openapi.yml
- filename: copper-people-api-openapi.yml
  format: yaml
  label: Copper People API
  slug: copper-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/openapi/copper-people-api-openapi.yml
- filename: copper-tasks-api-openapi.yml
  format: yaml
  label: Copper Tasks API
  slug: copper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/openapi/copper-tasks-api-openapi.yml
- filename: copper-webhooks-api-openapi.yml
  format: yaml
  label: Copper Webhooks API
  slug: copper-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/openapi/copper-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "rapidssl.com"
  - 0 issue "www.digicert.com"
  - 0 iodef "mailto:ops@copper.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: copper.com
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.copper.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: developer.copper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.copper.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Copper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Copper, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Copper
provider_slug: copper
slug: copper-domain-security
source_filename: copper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.copper.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\n- host: developer.copper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\n- host: api.copper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: copper.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 iodef \"mailto:ops@copper.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/security/copper-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Activities
- Companies
- Contact Relationship Management
- Contacts
- CRM
- Google Workspace
- Leads
- Opportunities
- People
- Project
- Sales
- Task
---

---
api_specs:
- filename: nimble-openapi-original.yml
  format: yaml
  label: Nimble REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/_original/nimble-openapi-original.yml
- filename: nimble-activities-api-openapi.yml
  format: yaml
  label: Nimble Activities API
  slug: nimble-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-activities-api-openapi.yml
- filename: nimble-contacts-api-openapi.yml
  format: yaml
  label: Nimble Contacts API
  slug: nimble-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-api-openapi.yml
- filename: nimble-contacts-fields-api-openapi.yml
  format: yaml
  label: Nimble Contacts Fields API
  slug: nimble-contacts-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-fields-api-openapi.yml
- filename: nimble-contacts-pipelines-api-openapi.yml
  format: yaml
  label: Nimble Contacts Pipelines API
  slug: nimble-contacts-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-pipelines-api-openapi.yml
- filename: nimble-deals-api-openapi.yml
  format: yaml
  label: Nimble Deals API
  slug: nimble-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-api-openapi.yml
- filename: nimble-deals-fields-api-openapi.yml
  format: yaml
  label: Nimble Deals Fields API
  slug: nimble-deals-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-fields-api-openapi.yml
- filename: nimble-deals-pipelines-api-openapi.yml
  format: yaml
  label: Nimble Deals Pipelines API
  slug: nimble-deals-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-pipelines-api-openapi.yml
- filename: nimble-deals-pipelines-fields-api-openapi.yml
  format: yaml
  label: Nimble Deals Pipelines Fields API
  slug: nimble-deals-pipelines-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-pipelines-fields-api-openapi.yml
- filename: nimble-leads-api-openapi.yml
  format: yaml
  label: Nimble Leads API
  slug: nimble-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-leads-api-openapi.yml
- filename: nimble-messages-api-openapi.yml
  format: yaml
  label: Nimble Messages API
  slug: nimble-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-messages-api-openapi.yml
- filename: nimble-tasks-api-openapi.yml
  format: yaml
  label: Nimble Tasks API
  slug: nimble-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-tasks-api-openapi.yml
- filename: nimble-users-api-openapi.yml
  format: yaml
  label: Nimble Users API
  slug: nimble-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:admin@nimble.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nimble.com
  spf: true
hosts:
- cert_expires: Sep 22 23:18:47 2026 GMT
  host: www.nimble.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:18:47 2026 GMT
  host: api.nimble.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:18:47 2026 GMT
  host: app.nimble.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nimble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nimble, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nimble
provider_slug: nimble
slug: nimble-domain-security
source_filename: nimble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: app.nimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: nimble.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:admin@nimble.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/security/nimble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Sales
- Contact Management
- Relationship Management
- Marketing Automation
- Pipeline Management
- Small Business
- Email Marketing
- Sales Automation
- Lead Management
---

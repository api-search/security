---
api_specs:
- filename: freshdesk-webhook-api-asyncapi.yml
  format: yaml
  label: Freshdesk Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/asyncapi/freshdesk-webhook-api-asyncapi.yml
- filename: freshdesk-agents-api-openapi.yml
  format: yaml
  label: freshdesk Agents API
  slug: freshdesk-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-agents-api-openapi.yml
- filename: freshdesk-business-hours-api-openapi.yml
  format: yaml
  label: freshdesk Business Hours API
  slug: freshdesk-business-hours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-business-hours-api-openapi.yml
- filename: freshdesk-companies-api-openapi.yml
  format: yaml
  label: freshdesk Companies API
  slug: freshdesk-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-companies-api-openapi.yml
- filename: freshdesk-contacts-api-openapi.yml
  format: yaml
  label: freshdesk Contacts API
  slug: freshdesk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-contacts-api-openapi.yml
- filename: freshdesk-conversations-api-openapi.yml
  format: yaml
  label: freshdesk Conversations API
  slug: freshdesk-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-conversations-api-openapi.yml
- filename: freshdesk-email-configs-api-openapi.yml
  format: yaml
  label: freshdesk Email Configs API
  slug: freshdesk-email-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-email-configs-api-openapi.yml
- filename: freshdesk-groups-api-openapi.yml
  format: yaml
  label: freshdesk Groups API
  slug: freshdesk-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-groups-api-openapi.yml
- filename: freshdesk-products-api-openapi.yml
  format: yaml
  label: freshdesk Products API
  slug: freshdesk-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-products-api-openapi.yml
- filename: freshdesk-roles-api-openapi.yml
  format: yaml
  label: freshdesk Roles API
  slug: freshdesk-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-roles-api-openapi.yml
- filename: freshdesk-satisfaction-ratings-api-openapi.yml
  format: yaml
  label: freshdesk Satisfaction Ratings API
  slug: freshdesk-satisfaction-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-satisfaction-ratings-api-openapi.yml
- filename: freshdesk-search-api-openapi.yml
  format: yaml
  label: freshdesk Search API
  slug: freshdesk-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-search-api-openapi.yml
- filename: freshdesk-sla-policies-api-openapi.yml
  format: yaml
  label: freshdesk SLA Policies API
  slug: freshdesk-sla-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-sla-policies-api-openapi.yml
- filename: freshdesk-solutions-api-openapi.yml
  format: yaml
  label: freshdesk Solutions API
  slug: freshdesk-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-solutions-api-openapi.yml
- filename: freshdesk-tickets-api-openapi.yml
  format: yaml
  label: freshdesk Tickets API
  slug: freshdesk-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-tickets-api-openapi.yml
- filename: freshdesk-time-entries-api-openapi.yml
  format: yaml
  label: freshdesk Time Entries API
  slug: freshdesk-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-time-entries-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freshdesk.com
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: developers.freshdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 17:44:14 2026 GMT
  host: yourdomain.freshdesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 17:44:14 2026 GMT
  host: support.freshdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freshdesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Freshdesk
provider_slug: freshdesk
slug: freshdesk-domain-security
source_filename: freshdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.freshdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourdomain.freshdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:44:14 2026 GMT\n  hsts: null\n- host: support.freshdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:44:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freshdesk.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/security/freshdesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---

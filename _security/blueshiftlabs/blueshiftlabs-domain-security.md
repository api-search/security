---
api_specs:
- filename: blueshiftlabs-blueshiftlabs-api-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Blueshiftlabs API
  slug: blueshiftlabs-blueshiftlabs-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-blueshiftlabs-api-api-openapi.yml
- filename: blueshiftlabs-campaigns-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Campaigns API
  slug: blueshiftlabs-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-campaigns-api-openapi.yml
- filename: blueshiftlabs-campaigns-json-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Campaigns.json API
  slug: blueshiftlabs-campaigns-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-campaigns-json-api-openapi.yml
- filename: blueshiftlabs-custom-user-lists-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Custom User Lists API
  slug: blueshiftlabs-custom-user-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-custom-user-lists-api-openapi.yml
- filename: blueshiftlabs-customer-group-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Customer Group API
  slug: blueshiftlabs-customer-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-customer-group-api-openapi.yml
- filename: blueshiftlabs-customers-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Customers API
  slug: blueshiftlabs-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-customers-api-openapi.yml
- filename: blueshiftlabs-emails-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Emails API
  slug: blueshiftlabs-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-emails-api-openapi.yml
- filename: blueshiftlabs-event-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Event API
  slug: blueshiftlabs-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-event-api-openapi.yml
- filename: blueshiftlabs-interests-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Interests API
  slug: blueshiftlabs-interests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-interests-api-openapi.yml
- filename: blueshiftlabs-list-api-openapi.yml
  format: yaml
  label: Blueshiftlabs List API
  slug: blueshiftlabs-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-list-api-openapi.yml
- filename: blueshiftlabs-live-activity-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Live Activity API
  slug: blueshiftlabs-live-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-live-activity-api-openapi.yml
- filename: blueshiftlabs-live-api-openapi.yml
  format: yaml
  label: Blueshiftlabs Live API
  slug: blueshiftlabs-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/openapi/blueshiftlabs-live-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blueshift.com
  spf: true
hosts:
- cert_expires: Dec 21 08:52:14 2026 GMT
  host: blueshift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blueshiftlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blueshiftlabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blueshiftlabs
provider_slug: blueshiftlabs
slug: blueshiftlabs-domain-security
source_filename: blueshiftlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blueshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 08:52:14 2026 GMT\n  hsts: false\ndomains:\n- domain: blueshift.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueshiftlabs/refs/heads/main/security/blueshiftlabs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Marketing
- Customer Engagement
- Consumer
---

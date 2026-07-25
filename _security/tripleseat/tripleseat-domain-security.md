---
api_specs:
- filename: tripleseat-accounts-api-openapi.yml
  format: yaml
  label: Tripleseat Accounts API
  slug: tripleseat-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-accounts-api-openapi.yml
- filename: tripleseat-contacts-api-openapi.yml
  format: yaml
  label: Tripleseat Contacts API
  slug: tripleseat-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-contacts-api-openapi.yml
- filename: tripleseat-events-api-openapi.yml
  format: yaml
  label: Tripleseat Events API
  slug: tripleseat-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-events-api-openapi.yml
- filename: tripleseat-leads-api-openapi.yml
  format: yaml
  label: Tripleseat Leads API
  slug: tripleseat-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-leads-api-openapi.yml
- filename: tripleseat-locations-api-openapi.yml
  format: yaml
  label: Tripleseat Locations API
  slug: tripleseat-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-locations-api-openapi.yml
- filename: tripleseat-sites-api-openapi.yml
  format: yaml
  label: Tripleseat Sites API
  slug: tripleseat-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-sites-api-openapi.yml
- filename: tripleseat-users-api-openapi.yml
  format: yaml
  label: Tripleseat Users API
  slug: tripleseat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tripleseat.com
  spf: true
hosts:
- cert_expires: Sep 30 23:15:04 2026 GMT
  host: tripleseat.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:39:55 2026 GMT
  host: support.tripleseat.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: api.tripleseat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tripleseat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tripleseat, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tripleseat
provider_slug: tripleseat
slug: tripleseat-domain-security
source_filename: tripleseat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripleseat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:15:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.tripleseat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:39:55 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.tripleseat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tripleseat.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/security/tripleseat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Events
- Catering
- Leads
- Webhooks
- Sales
---

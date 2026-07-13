---
api_specs:
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Accounts API
  slug: neonone-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Households API
  slug: neonone-households-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Donations API
  slug: neonone-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Campaigns API
  slug: neonone-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Memberships API
  slug: neonone-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Events API
  slug: neonone-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Custom Fields API
  slug: neonone-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Orders & Store API
  slug: neonone-orders-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Volunteers API
  slug: neonone-volunteers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Webhooks API
  slug: neonone-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: neonone.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neoncrm.com
  spf: true
hosts:
- cert_expires: Aug 24 18:29:21 2026 GMT
  host: neonone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:22:25 2026 GMT
  host: developer.neoncrm.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.neoncrm.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Neonone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neon One, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Neon One
provider_slug: neonone
slug: neonone-domain-security
source_filename: neonone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neonone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:29:21 2026 GMT\n  hsts: null\n- host: developer.neoncrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:22:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.neoncrm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: neonone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: neoncrm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/security/neonone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nonprofit
- CRM
- Fundraising
- Donor Management
- Membership Management
- Events
---

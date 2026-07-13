---
api_specs:
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Club Members API
  slug: virtuagym-club-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Club Employees API
  slug: virtuagym-club-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Memberships API
  slug: virtuagym-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Billing API
  slug: virtuagym-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Visits API
  slug: virtuagym-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Events API
  slug: virtuagym-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Coaching Workouts API
  slug: virtuagym-coaching-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: virtuagym.com
  spf: true
  spf_policy: ~all
  spf_record: v=spf1 include:_spf.virtuagym.com include:salesforce.com include:spf.mandrillapp.com include:servers.mcsv.net include:_spf.google.com ~all
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api.virtuagym.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: virtuagym.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.virtuagym.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 600
  https: true
  note: Redirects (HTTP 301) to the apex / business host.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virtuagym Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtuagym, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Virtuagym
provider_slug: virtuagym
slug: virtuagym-domain-security
source_filename: virtuagym-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.virtuagym.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 600\n  hsts_include_subdomains: true\n- host: virtuagym.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 600\n  hsts_include_subdomains: true\n- host: www.virtuagym.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 600\n  hsts_include_subdomains: true\n  note: Redirects (HTTP 301) to the apex / business host.\ndomains:\n- domain: virtuagym.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '~all'\n  spf_record: 'v=spf1 include:_spf.virtuagym.com include:salesforce.com include:spf.mandrillapp.com include:servers.mcsv.net include:_spf.google.com ~all'\n  dmarc: true\n  dmarc_policy: none\nnotes:\
  \ >-\n  All three probed hosts serve HTTPS over TLS 1.3 with valid certificates\n  expiring Jan 4 2027 and enforce HSTS, though with a notably short max-age of\n  600 seconds (10 minutes) rather than a long-lived policy. SPF is published with\n  a soft-fail (~all) covering Salesforce, Mandrill, Mailchimp, and Google as\n  senders; DMARC is present but set to p=none (monitor only, not enforcing). No\n  CAA records were observed on virtuagym.com and DNSSEC is not enabled. The\n  Public API is served from api.virtuagym.com, which requires HTTPS for all\n  requests.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/security/virtuagym-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Health Club Management
- Gym Management
- Coaching
- Membership Management
- Fitness Software
- Wellness
- Scheduling
- SaaS
---

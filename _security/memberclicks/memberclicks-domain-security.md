---
api_specs:
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Profiles API
  slug: memberclicks-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Profile Search API
  slug: memberclicks-profile-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Attributes API
  slug: memberclicks-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Member Types and Statuses API
  slug: memberclicks-member-types-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Groups API
  slug: memberclicks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Events API
  slug: memberclicks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Continuing Education API
  slug: memberclicks-continuing-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memberclicks.com
  spf: true
hosts:
- cert_expires: Oct  1 17:31:22 2026 GMT
  host: memberclicks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:44:36 2026 GMT
  host: help.memberclicks.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memberclicks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MemberClicks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MemberClicks
provider_slug: memberclicks
slug: memberclicks-domain-security
source_filename: memberclicks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memberclicks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:31:22 2026 GMT\n  hsts: false\n- host: help.memberclicks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:44:36 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: memberclicks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/security/memberclicks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Membership Management
- Association Management
- AMS
- Nonprofit
- Events
- CRM
- Personify
---

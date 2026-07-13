---
api_specs:
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Contacts API
  slug: growthzone-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Memberships API
  slug: growthzone-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Groups & Directory API
  slug: growthzone-groups-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Scheduled Billing API
  slug: growthzone-scheduled-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Certifications API
  slug: growthzone-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Events API
  slug: growthzone-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone OAuth / OpenID Connect (SSO) API
  slug: growthzone-oauth-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: growthzone.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: growthzoneapp.com
  spf: true
hosts:
- cert_expires: Oct  2 00:18:29 2026 GMT
  host: www.growthzone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 01:14:54 2026 GMT
  host: integration.growthzone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 12:05:35 2026 GMT
  host: documentation.growthzoneapp.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Growthzone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GrowthZone, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GrowthZone
provider_slug: growthzone
slug: growthzone-domain-security
source_filename: growthzone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.growthzone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:18:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integration.growthzone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:14:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.growthzoneapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 12:05:35 2026 GMT\n  hsts: false\ndomains:\n- domain: growthzone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: growthzoneapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/security/growthzone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Association Management
- AMS
- Membership Management
- Chambers of Commerce
- ChamberMaster
- Member Directory
- Events
- Billing
---

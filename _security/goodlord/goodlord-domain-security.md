---
api_specs:
- filename: goodlord-agent-api-openapi.yml
  format: yaml
  label: Goodlord Agent API
  slug: goodlord-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-agent-api-openapi.yml
- filename: goodlord-application-api-openapi.yml
  format: yaml
  label: Goodlord Application API
  slug: goodlord-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-application-api-openapi.yml
- filename: goodlord-authentication-api-openapi.yml
  format: yaml
  label: Goodlord Authentication API
  slug: goodlord-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-authentication-api-openapi.yml
- filename: goodlord-company-api-openapi.yml
  format: yaml
  label: Goodlord Company API
  slug: goodlord-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-company-api-openapi.yml
- filename: goodlord-file-api-openapi.yml
  format: yaml
  label: Goodlord File API
  slug: goodlord-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-file-api-openapi.yml
- filename: goodlord-insuranceclaim-api-openapi.yml
  format: yaml
  label: Goodlord Insurance Claim API
  slug: goodlord-insuranceclaim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-insuranceclaim-api-openapi.yml
- filename: goodlord-media-api-openapi.yml
  format: yaml
  label: Goodlord Media API
  slug: goodlord-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-media-api-openapi.yml
- filename: goodlord-payment-api-openapi.yml
  format: yaml
  label: Goodlord Payment API
  slug: goodlord-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-payment-api-openapi.yml
- filename: goodlord-rentschedule-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule API
  slug: goodlord-rentschedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedule-api-openapi.yml
- filename: goodlord-rentschedulerow-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row API
  slug: goodlord-rentschedulerow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerow-api-openapi.yml
- filename: goodlord-rentschedulerowpostdto-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row Post Dto API
  slug: goodlord-rentschedulerowpostdto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerowpostdto-api-openapi.yml
- filename: goodlord-rentschedulerowupdate-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row Update API
  slug: goodlord-rentschedulerowupdate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerowupdate-api-openapi.yml
- filename: goodlord-role-api-openapi.yml
  format: yaml
  label: Goodlord Role API
  slug: goodlord-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-role-api-openapi.yml
- filename: goodlord-rolegroup-api-openapi.yml
  format: yaml
  label: Goodlord Role Group API
  slug: goodlord-rolegroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rolegroup-api-openapi.yml
- filename: goodlord-subject-api-openapi.yml
  format: yaml
  label: Goodlord Subject API
  slug: goodlord-subject-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-subject-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodlord.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodlord.co
  spf: true
hosts:
- cert_expires: Oct  2 13:41:03 2026 GMT
  host: www.goodlord.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 06:46:24 2026 GMT
  host: portal.goodlord.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.goodoverlord.com
  https: false
kind: domain-security
layout: security
method: probed
name: Goodlord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodlord, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Goodlord
provider_slug: goodlord
slug: goodlord-domain-security
source_filename: goodlord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodlord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:41:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.goodlord.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 06:46:24 2026 GMT\n  hsts: false\n- host: api.goodoverlord.com\n  https: false\ndomains:\n- domain: goodlord.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: goodlord.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/security/goodlord-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Management
- Rentals
- Lettings
- Tenant Referencing
- Tenancy Management
- Insurance
- Payments
---

---
api_specs:
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center People API
  slug: planning-center-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Services API
  slug: planning-center-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Giving API
  slug: planning-center-giving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Groups API
  slug: planning-center-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Check-Ins API
  slug: planning-center-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Calendar API
  slug: planning-center-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Registrations API
  slug: planning-center-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Publishing API
  slug: planning-center-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Webhooks API
  slug: planning-center-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: planningcenter.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: planning.center
  spf: true
hosts:
- cert_expires: Aug 16 22:04:08 2026 GMT
  host: www.planningcenter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: developer.planning.center
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.planningcenteronline.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planning Center Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Planning Center, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Planning Center
provider_slug: planning-center
slug: planning-center-domain-security
source_filename: planning-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.planningcenter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 22:04:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.planning.center\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.planningcenteronline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: planningcenter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: planning.center\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/security/planning-center-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Church Management
- ChMS
- Faith
- Giving
- Events
- Scheduling
- People
- Nonprofit
---

---
api_specs:
- filename: sprig-purge-api-openapi.yml
  format: yaml
  label: Sprig Purge API
  slug: sprig-purge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/openapi/sprig-purge-api-openapi.yml
- filename: sprig-responses-api-openapi.yml
  format: yaml
  label: Sprig Responses API
  slug: sprig-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/openapi/sprig-responses-api-openapi.yml
- filename: sprig-surveys-api-openapi.yml
  format: yaml
  label: Sprig Surveys API
  slug: sprig-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/openapi/sprig-surveys-api-openapi.yml
- filename: sprig-themes-api-openapi.yml
  format: yaml
  label: Sprig Themes API
  slug: sprig-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/openapi/sprig-themes-api-openapi.yml
- filename: sprig-users-api-openapi.yml
  format: yaml
  label: Sprig Users API
  slug: sprig-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/openapi/sprig-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: userleap.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sprig.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: userleap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.sprig.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Sprig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sprig, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sprig
provider_slug: sprig
slug: sprig-domain-security
source_filename: sprig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userleap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sprig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: userleap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sprig.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/security/sprig-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Product Research
- Surveys
- User Insights
- Customer Experience
- Analytics
- Product Analytics
- Artificial Intelligence
- Software-as-a-Service
---

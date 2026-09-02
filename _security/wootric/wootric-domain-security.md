---
api_specs:
- filename: wootric-declines-api-openapi.yml
  format: yaml
  label: Wootric Declines API
  slug: wootric-declines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-declines-api-openapi.yml
- filename: wootric-email-surveys-api-openapi.yml
  format: yaml
  label: Wootric Email Surveys API
  slug: wootric-email-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-email-surveys-api-openapi.yml
- filename: wootric-end-users-api-openapi.yml
  format: yaml
  label: Wootric End Users API
  slug: wootric-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-end-users-api-openapi.yml
- filename: wootric-metrics-api-openapi.yml
  format: yaml
  label: Wootric Metrics API
  slug: wootric-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-metrics-api-openapi.yml
- filename: wootric-responses-api-openapi.yml
  format: yaml
  label: Wootric Responses API
  slug: wootric-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-responses-api-openapi.yml
- filename: wootric-segments-api-openapi.yml
  format: yaml
  label: Wootric Segments API
  slug: wootric-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-segments-api-openapi.yml
- filename: wootric-settings-api-openapi.yml
  format: yaml
  label: Wootric Settings API
  slug: wootric-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-settings-api-openapi.yml
- filename: wootric-survey-templates-api-openapi.yml
  format: yaml
  label: Wootric Survey Templates API
  slug: wootric-survey-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-survey-templates-api-openapi.yml
description: ''
domains:
- caa:
  - wp.wpenginepowered.com.
  dmarc: false
  dnssec: true
  domain: wootric.com
  spf: true
hosts:
- cert_expires: Sep  5 01:35:10 2026 GMT
  host: wootric.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 01:10:49 2026 GMT
  host: docs.wootric.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 00:02:40 2026 GMT
  host: api.wootric.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wootric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wootric, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Wootric
provider_slug: wootric
slug: wootric-domain-security
source_filename: wootric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wootric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 01:35:10 2026 GMT\n  hsts: false\n- host: docs.wootric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:10:49 2026 GMT\n  hsts: false\n- host: api.wootric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 00:02:40 2026 GMT\n  hsts: null\ndomains:\n- domain: wootric.com\n  dnssec: true\n  caa:\n  - wp.wpenginepowered.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/security/wootric-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Customer Experience
- NPS
- CSAT
- CES
- Customer Satisfaction
- Customer Effort Score
- Surveys
- Feedback
- Voice of the Customer
---

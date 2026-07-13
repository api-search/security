---
api_specs:
- filename: sift-events-api-openapi.yml
  format: yaml
  label: Sift Events API
  slug: sift-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-events-api-openapi.yml
- filename: sift-decisions-api-openapi.yml
  format: yaml
  label: Sift Decisions API
  slug: sift-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-decisions-api-openapi.yml
- filename: sift-score-api-openapi.yml
  format: yaml
  label: Sift Score API
  slug: sift-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-score-api-openapi.yml
- filename: sift-verification-api-openapi.yml
  format: yaml
  label: Sift Verification API
  slug: sift-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-verification-api-openapi.yml
- filename: sift-workflows-api-openapi.yml
  format: yaml
  label: Sift Workflows API
  slug: sift-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-workflows-api-openapi.yml
- filename: sift-labels-api-openapi.yml
  format: yaml
  label: Sift Labels API
  slug: sift-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-labels-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sift.com
  spf: true
hosts:
- cert_expires: Sep  6 01:38:22 2026 GMT
  host: sift.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: developers.sift.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: api.sift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sift Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sift, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sift
provider_slug: sift-com
slug: sift-com-domain-security
source_filename: sift-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:38:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.sift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/security/sift-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Trust And Safety
- Risk Scoring
- Identity Verification
- Chargebacks
- Account Takeover
- Content Abuse
---

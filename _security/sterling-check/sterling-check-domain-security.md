---
api_specs:
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Screenings API
  slug: sterling-check-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Candidates API
  slug: sterling-check-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Packages API
  slug: sterling-check-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Reports API
  slug: sterling-check-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Invites API
  slug: sterling-check-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Webhooks API
  slug: sterling-check-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sterlingcheck.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sterlingcheck.app
  spf: true
hosts:
- cert_expires: Sep  2 11:19:50 2026 GMT
  host: www.sterlingcheck.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 17:53:07 2026 GMT
  host: apidocs.sterlingcheck.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.sterlingcheck.app
  https: false
kind: domain-security
layout: security
method: probed
name: Sterling Check Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sterling, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sterling
provider_slug: sterling-check
slug: sterling-check-domain-security
source_filename: sterling-check-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sterlingcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 11:19:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.sterlingcheck.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:53:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sterlingcheck.app\n  https: false\ndomains:\n- domain: sterlingcheck.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sterlingcheck.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/security/sterling-check-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Background Screening
- Identity Verification
- Background Check
- HR Tech
- Compliance
- Gated API
---

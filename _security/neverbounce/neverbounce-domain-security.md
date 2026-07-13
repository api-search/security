---
api_specs:
- filename: neverbounce-openapi.yml
  format: yaml
  label: NeverBounce API v4
  slug: v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: neverbounce.com
  spf: true
hosts:
- cert_expires: Oct  3 07:14:34 2026 GMT
  host: www.neverbounce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:45:02 2026 GMT
  host: developers.neverbounce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:14:34 2026 GMT
  host: api.neverbounce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neverbounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NeverBounce, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NeverBounce
provider_slug: neverbounce
slug: neverbounce-domain-security
source_filename: neverbounce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neverbounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:14:34 2026 GMT\n  hsts: null\n- host: developers.neverbounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:45:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.neverbounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:14:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: neverbounce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/security/neverbounce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Verification
- Email Validation
- Email Hygiene
- Deliverability
- Marketing
- List Cleaning
- ZeroBounce
---

---
api_specs:
- filename: clearspeed-default-api-openapi.yml
  format: yaml
  label: Clearspeed Default API
  slug: clearspeed-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearspeed/refs/heads/main/openapi/clearspeed-default-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clearspeed.com
  spf: true
hosts:
- cert_expires: Aug 31 19:00:55 2026 GMT
  host: www.clearspeed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 12:15:56 2026 GMT
  host: developer.clearspeed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 09:49:34 2026 GMT
  host: api.us.clearspeed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clearspeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clearspeed, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clearspeed
provider_slug: clearspeed
slug: clearspeed-domain-security
source_filename: clearspeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearspeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:00:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.clearspeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 12:15:56 2026 GMT\n  hsts: false\n- host: api.us.clearspeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:49:34 2026 GMT\n  hsts: null\ndomains:\n- domain: clearspeed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearspeed/refs/heads/main/security/clearspeed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Risk Assessment
- Fraud Detection
- Voice Analytics
- Artificial Intelligence
- Insurance
- Identity Verification
- Screening
- Security
---

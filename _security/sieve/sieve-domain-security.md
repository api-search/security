---
api_specs:
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Jobs Push API
  slug: sieve-jobs-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Jobs Status API
  slug: sieve-jobs-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Functions API
  slug: sieve-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Webhooks API
  slug: sieve-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sievedata.com
  spf: true
hosts:
- cert_expires: Sep 29 20:41:26 2026 GMT
  host: www.sievedata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.sievedata.com
  https: false
- host: mango.sievedata.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sieve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sieve, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sieve
provider_slug: sieve
slug: sieve-domain-security
source_filename: sieve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sievedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:41:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sievedata.com\n  https: false\n- host: mango.sievedata.com\n  https: false\ndomains:\n- domain: sievedata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/security/sieve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Video
- Audio
- Media Processing
- Async Jobs
---

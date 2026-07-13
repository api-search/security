---
api_specs:
- filename: coconut-openapi.yml
  format: yaml
  label: Coconut Jobs API
  slug: coconut-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coconut/refs/heads/main/openapi/coconut-openapi.yml
- filename: coconut-openapi.yml
  format: yaml
  label: Coconut Metadata API
  slug: coconut-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coconut/refs/heads/main/openapi/coconut-openapi.yml
- filename: coconut-openapi.yml
  format: yaml
  label: Coconut Webhooks API
  slug: coconut-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coconut/refs/heads/main/openapi/coconut-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coconut.co
  spf: true
hosts:
- cert_expires: Aug 16 11:48:27 2026 GMT
  host: www.coconut.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 20:11:26 2026 GMT
  host: docs.coconut.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.coconut.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Coconut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coconut, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Coconut
provider_slug: coconut
slug: coconut-domain-security
source_filename: coconut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coconut.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:48:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.coconut.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 20:11:26 2026 GMT\n  hsts: false\n- host: api.coconut.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coconut.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coconut/refs/heads/main/security/coconut-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Video
- Audio
- Encoding
- Transcoding
- Media
---

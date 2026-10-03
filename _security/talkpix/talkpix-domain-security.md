---
api_specs:
- filename: talkpix-estimate-api-openapi.yml
  format: yaml
  label: TalkPix API Estimate API
  slug: talkpix-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpix/refs/heads/main/openapi/talkpix-estimate-api-openapi.yml
- filename: talkpix-me-api-openapi.yml
  format: yaml
  label: TalkPix API Me API
  slug: talkpix-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpix/refs/heads/main/openapi/talkpix-me-api-openapi.yml
- filename: talkpix-talkpix-api-api-api-openapi.yml
  format: yaml
  label: TalkPix API TalkPix API API
  slug: talkpix-talkpix-api-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpix/refs/heads/main/openapi/talkpix-talkpix-api-api-api-openapi.yml
- filename: talkpix-uploads-api-openapi.yml
  format: yaml
  label: TalkPix API Uploads API
  slug: talkpix-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpix/refs/heads/main/openapi/talkpix-uploads-api-openapi.yml
- filename: talkpix-videos-api-openapi.yml
  format: yaml
  label: TalkPix API Videos API
  slug: talkpix-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpix/refs/heads/main/openapi/talkpix-videos-api-openapi.yml
- filename: talkpix-voices-api-openapi.yml
  format: yaml
  label: TalkPix API Voices API
  slug: talkpix-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpix/refs/heads/main/openapi/talkpix-voices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: talkpix.ai
  spf: true
hosts:
- cert_expires: Nov 21 15:47:16 2026 GMT
  host: www.talkpix.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Talkpix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TalkPix API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TalkPix API
provider_slug: talkpix
slug: talkpix-domain-security
source_filename: talkpix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.talkpix.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 15:47:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: talkpix.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkpix/refs/heads/main/security/talkpix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Video
- Talking Photo
- Media
---

---
api_specs:
- filename: tl-dv-meetings-api-openapi.yml
  format: yaml
  label: tl;dv Meetings API
  slug: tl-dv-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-meetings-api-openapi.yml
- filename: tl-dv-notes-api-openapi.yml
  format: yaml
  label: tl;dv Notes API
  slug: tl-dv-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-notes-api-openapi.yml
- filename: tl-dv-system-api-openapi.yml
  format: yaml
  label: tl;dv System API
  slug: tl-dv-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-system-api-openapi.yml
- filename: tl-dv-transcripts-api-openapi.yml
  format: yaml
  label: tl;dv Transcripts API
  slug: tl-dv-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-transcripts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "Cloudflare Inc ECC CA-3"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tldv.io
  spf: true
hosts:
- cert_expires: Sep 27 04:06:04 2026 GMT
  host: tldv.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 04:06:04 2026 GMT
  host: doc.tldv.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 04:06:04 2026 GMT
  host: pasta.tldv.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tl Dv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tl;dv, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: tl;dv
provider_slug: tl-dv
slug: tl-dv-domain-security
source_filename: tl-dv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tldv.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:06:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: doc.tldv.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:06:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: pasta.tldv.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:06:04 2026 GMT\n  hsts: null\ndomains:\n- domain: tldv.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"Cloudflare Inc ECC CA-3\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/security/tl-dv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Meetings
- Transcription
- Note Taking
- Conversation Intelligence
- Productivity
- Video
- Webhook
---

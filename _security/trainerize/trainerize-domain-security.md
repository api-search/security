---
api_specs:
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Clients API
  slug: trainerize-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Training Programs API
  slug: trainerize-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Client Data API
  slug: trainerize-client-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Messaging API
  slug: trainerize-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Webhooks API
  slug: trainerize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trainerize.com
  spf: true
  spf_policy: -all
  spf_record: v=spf1 include:spf.recurly.com include:spf.mandrillapp.com include:mail.zendesk.com include:_spf.google.com include:us._netblocks.mimecast.com include:spf.protection.outlook.com ip4:192.54.252.0/24 ip4:168.215.168.0/24 -all
hosts:
- cert_expires: Oct  6 21:06:58 2026 GMT
  host: www.trainerize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Marketing / app site. Fronted by Cloudflare.
  server: Cloudflare (fronting)
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: trainerize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Apex redirects (301) to www.
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.trainerize.com
  hsts: false
  https: true
  note: Live API host. Root returns 403 Forbidden; the /v03 version prefix responds 200. No HSTS header observed on the API host. Requires provisioned credentials (Studio/Enterprise).
  server: Microsoft-IIS/10.0 (ASP.NET Web API, behind Cloudflare + AWS ELB)
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:39:36 2026 GMT
  host: help.trainerize.com
  hsts: true
  hsts_max_age: 259200
  https: true
  note: Zendesk-hosted help center (CNAME to trainerize.zendesk.com). Returns 403 to automated fetchers.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trainerize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ABC Trainerize, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ABC Trainerize
provider_slug: trainerize
slug: trainerize-domain-security
source_filename: trainerize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trainerize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:06:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: Cloudflare (fronting)\n  note: Marketing / app site. Fronted by Cloudflare.\n- host: trainerize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Apex redirects (301) to www.\n- host: api.trainerize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n  server: Microsoft-IIS/10.0 (ASP.NET Web API, behind Cloudflare + AWS ELB)\n  note: >-\n    Live API host. Root returns 403 Forbidden; the /v03 version prefix responds\n    200. No HSTS header observed on the API host. Requires provisioned\n    credentials (Studio/Enterprise).\n- host: help.trainerize.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Sep 23 23:39:36 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  note: Zendesk-hosted help center (CNAME to trainerize.zendesk.com). Returns 403 to automated fetchers.\ndomains:\n- domain: trainerize.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  spf_record: 'v=spf1 include:spf.recurly.com include:spf.mandrillapp.com include:mail.zendesk.com include:_spf.google.com include:us._netblocks.mimecast.com include:spf.protection.outlook.com ip4:192.54.252.0/24 ip4:168.215.168.0/24 -all'\n  dmarc: true\n  dmarc_policy: none\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/security/trainerize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Personal Training
- Coaching
- Fitness Software
- Client Management
- SaaS
---

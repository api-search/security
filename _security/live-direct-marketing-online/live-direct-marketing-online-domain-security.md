---
api_specs:
- filename: live-direct-marketing-online-ldm-v3-openapi.json
  format: json
  label: LDM v3 API
  slug: ldm-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-direct-marketing-online/refs/heads/main/openapi/live-direct-marketing-online-ldm-v3-openapi.json
- filename: live-direct-marketing-online-inbox-check-openapi.json
  format: json
  label: Inbox Check API
  slug: inbox-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-direct-marketing-online/refs/heads/main/openapi/live-direct-marketing-online-inbox-check-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:welcome@live-direct-marketing.online"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: live-direct-marketing.online
  spf: true
hosts:
- cert_expires: Oct 24 00:37:58 2026 GMT
  host: live-direct-marketing.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 19:09:05 2026 GMT
  host: developers.live-direct-marketing.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 19:08:37 2026 GMT
  host: api.live-direct-marketing.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Live Direct Marketing Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Live Direct Marketing, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Live Direct Marketing
provider_slug: live-direct-marketing-online
slug: live-direct-marketing-online-domain-security
source_filename: live-direct-marketing-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: live-direct-marketing.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 00:37:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.live-direct-marketing.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 19:09:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.live-direct-marketing.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 19:08:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: live-direct-marketing.online\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:welcome@live-direct-marketing.online\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/live-direct-marketing-online/refs/heads/main/security/live-direct-marketing-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Email Deliverability
- Sales & marketing automation
- CRM
- Lead Management
- Cold Outreach
- agent-native
- MCP
- A2A
- Webhook
- B2B
---

---
api_specs:
- filename: tgatlas-openapi.json
  format: json
  label: ChannelIndex Telegram Channel Data API
  slug: channelindex-telegram-channel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tgatlas/refs/heads/main/openapi/tgatlas-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Dec 13 16:28:19 2026 GMT
  host: channelindex.starnikovoleg.workers.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: telegram155.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Tgatlas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChannelIndex (tgAtlas), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChannelIndex (tgAtlas)
provider_slug: tgatlas
slug: tgatlas-domain-security
source_filename: tgatlas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: channelindex.starnikovoleg.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 16:28:19 2026 GMT\n  hsts: false\n- host: telegram155.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tgatlas/refs/heads/main/security/tgatlas-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Telegram
- Public Channels
- Social-Media
- Social Monitoring
- Messaging
- Directory
- Search
- Analytics
- OSINT
- Market Research
- AI-agent context
---

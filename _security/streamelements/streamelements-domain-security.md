---
api_specs:
- filename: streamelements-openapi-original.yml
  format: yaml
  label: StreamElements API
  slug: streamelements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamelements/refs/heads/main/openapi/streamelements-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: streamelements.com
  spf: true
hosts:
- cert_expires: Oct 12 03:24:58 2026 GMT
  host: api.streamelements.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Streamelements Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StreamElements, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: StreamElements
provider_slug: streamelements
slug: streamelements-domain-security
source_filename: streamelements-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.streamelements.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:24:58 2026 GMT\n  hsts: null\ndomains:\n- domain: streamelements.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamelements/refs/heads/main/security/streamelements-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Live Streaming
- Creator Economy
- Overlays
- Chatbot
- Monetization
- Donations
- Loyalty Points
- Giveaways
- Video
- Twitch
- YouTube
- Real-Time
- WebSockets
- Webhooks
- REST
---

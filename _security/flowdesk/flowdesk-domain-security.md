---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: flowdesk.co
  spf: true
hosts:
- cert_expires: Sep 25 12:28:30 2026 GMT
  host: www.flowdesk.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 00:26:51 2026 GMT
  host: docs.flowdesk.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 00:26:51 2026 GMT
  host: api.flowdesk.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flowdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowdesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Flowdesk
provider_slug: flowdesk
slug: flowdesk-domain-security
source_filename: flowdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flowdesk.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:28:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flowdesk.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:26:51 2026 GMT\n  hsts: false\n- host: api.flowdesk.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:26:51 2026 GMT\n  hsts: null\ndomains:\n- domain: flowdesk.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowdesk/refs/heads/main/security/flowdesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Crypto
- Digital Assets
- Trading
- Liquidity
- Market Maker
- OTC
- WebSocket
---

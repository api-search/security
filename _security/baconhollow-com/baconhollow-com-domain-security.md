---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: baconhollow.com
  spf: false
hosts:
- cert_expires: Nov 18 01:41:07 2026 GMT
  host: baconhollow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Baconhollow Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bot Hub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bot Hub
provider_slug: baconhollow-com
slug: baconhollow-com-domain-security
source_filename: baconhollow-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baconhollow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 01:41:07 2026 GMT\n  hsts: null\ndomains:\n- domain: baconhollow.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baconhollow-com/refs/heads/main/security/baconhollow-com-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Agents
- A2A
- Autonomous Agents
- Prediction Markets
- Kalshi
- Trading Signals
- Weather
- agent-native
---

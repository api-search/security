---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simulmedia.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: playerwon.com
  spf: true
hosts:
- cert_expires: Oct  6 03:43:52 2026 GMT
  host: simulmedia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 18:18:31 2026 GMT
  host: www.playerwon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 02:58:58 2026 GMT
  host: game.simulmedia-apis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simulmedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simulmedia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Simulmedia
provider_slug: simulmedia
slug: simulmedia-domain-security
source_filename: simulmedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simulmedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.playerwon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:18:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: game.simulmedia-apis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 02:58:58 2026 GMT\n  hsts: null\ndomains:\n- domain: simulmedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: playerwon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simulmedia/refs/heads/main/security/simulmedia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Television
- Connected TV
- Games
- AdTech
- Rewarded Video
- Media Buying
---

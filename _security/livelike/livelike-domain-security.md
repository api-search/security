---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: livelike.com
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: livelikecdn.com
  spf: false
hosts:
- cert_expires: Oct 18 01:16:26 2026 GMT
  host: www.livelike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:17:51 2026 GMT
  host: docs.livelike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: cf-blast.livelikecdn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Livelike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveLike, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LiveLike
provider_slug: livelike
slug: livelike-domain-security
source_filename: livelike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.livelike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:16:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.livelike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:17:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cf-blast.livelikecdn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: livelike.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: livelikecdn.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livelike/refs/heads/main/security/livelike-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fan Engagement
- Live Streaming
- Interactive Video
- Chat
- Gamification
- Widgets
- Sports
- Media
---

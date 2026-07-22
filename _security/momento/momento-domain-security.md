---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gomomento.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: momentohq.com
  spf: true
hosts:
- cert_expires: Sep 22 01:54:49 2026 GMT
  host: www.gomomento.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 20:11:19 2026 GMT
  host: docs.momentohq.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 15:35:18 2026 GMT
  host: api.cache.cell-1-ap-south-1-1.prod.a.momentohq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Momento Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Momento, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Momento
provider_slug: momento
slug: momento-domain-security
source_filename: momento-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gomomento.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:54:49 2026 GMT\n  hsts: false\n- host: docs.momentohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:11:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.cache.cell-1-ap-south-1-1.prod.a.momentohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:35:18 2026 GMT\n  hsts: null\ndomains:\n- domain: gomomento.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: momentohq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momento/refs/heads/main/security/momento-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Infrastructure
- Caching
- Serverless
- Cache
- Pub/Sub
- Messaging
- Event Bus
- Leaderboards
- Real Time
- gRPC
- Developer Tools
---

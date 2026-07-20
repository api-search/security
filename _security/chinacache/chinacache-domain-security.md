---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edgenext.com
  spf: true
hosts:
- cert_expires: Oct 15 02:48:03 2026 GMT
  host: www.edgenext.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: docs.edgenext.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: api.edgenext.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chinacache Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChinaCache (EdgeNext), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChinaCache (EdgeNext)
provider_slug: chinacache
slug: chinacache-domain-security
source_filename: chinacache-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.edgenext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:48:03 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.edgenext.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.edgenext.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: edgenext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chinacache/refs/heads/main/security/chinacache-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CDN
- Content Delivery Network
- Edge Computing
- Cloud Security
- DDoS Protection
- WAF
- Media Delivery
- Networking
- China
---

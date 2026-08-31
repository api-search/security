---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tvscientific.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tvscientific.app
  spf: true
hosts:
- cert_expires: Sep 20 00:38:26 2026 GMT
  host: tvscientific.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 08:55:49 2026 GMT
  host: status.tvscientific.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.tvscientific.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tvscientific Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tvscientific, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tvscientific
provider_slug: tvscientific
slug: tvscientific-domain-security
source_filename: tvscientific-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tvscientific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:38:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.tvscientific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 08:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.tvscientific.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tvscientific.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tvscientific.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvscientific/refs/heads/main/security/tvscientific-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Connected TV
- CTV
- Streaming
- Performance Marketing
- AdTech
- Measurements
- Campaign Management
- Real Time Bidding
- Attribution
---

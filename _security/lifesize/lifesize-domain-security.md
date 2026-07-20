---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lifesize.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lifesizecloud.com
  spf: true
hosts:
- cert_expires: Oct  8 17:21:48 2026 GMT
  host: lifesize.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 00:30:15 2026 GMT
  host: support.lifesize.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: admin.lifesizecloud.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lifesize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lifesize, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lifesize
provider_slug: lifesize
slug: lifesize-domain-security
source_filename: lifesize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lifesize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:21:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.lifesize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:30:15 2026 GMT\n  hsts: false\n- host: admin.lifesizecloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lifesize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lifesizecloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifesize/refs/heads/main/security/lifesize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video Conferencing
- Communications
- Collaboration
- Meetings
- Unified Communications
- Video
- Contact Center
- Conference Room Systems
- Streaming
---

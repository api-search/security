---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wyze.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wyzecam.com
  spf: true
hosts:
- cert_expires: Sep  5 14:53:03 2026 GMT
  host: www.wyze.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:43:57 2026 GMT
  host: support.wyze.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.wyzecam.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wyze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wyze, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wyze
provider_slug: wyze
slug: wyze-domain-security
source_filename: wyze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wyze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 14:53:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: support.wyze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wyzecam.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wyze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wyzecam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyze/refs/heads/main/security/wyze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Home
- Internet of Things
- Home Security
- Cameras
- Consumer Electronics
- Home Automation
- Video
- Sensors
- Commerce
---

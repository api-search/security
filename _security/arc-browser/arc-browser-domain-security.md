---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arc.net
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Sep 28 11:00:16 2026 GMT
  host: arc.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: chromewebstore.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:44:18 2026 GMT
  host: resources.arc.net
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arc Browser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arc (The Browser Company), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arc (The Browser Company)
provider_slug: arc-browser
slug: arc-browser-domain-security
source_filename: arc-browser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arc.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: chromewebstore.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: false\n- host: resources.arc.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:44:18 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: arc.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arc-browser/refs/heads/main/security/arc-browser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser
- Consumer
- Chromium
- Boosts
- The Browser Company
---

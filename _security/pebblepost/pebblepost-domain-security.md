---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pebblepost.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pbbl.co
  spf: true
hosts:
- cert_expires: Sep 22 05:04:19 2026 GMT
  host: www.pebblepost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 11:12:48 2026 GMT
  host: docs.pebblepost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: cdn.pbbl.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pebblepost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PebblePost, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PebblePost
provider_slug: pebblepost
slug: pebblepost-domain-security
source_filename: pebblepost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pebblepost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pebblepost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:12:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cdn.pbbl.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pebblepost.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pbbl.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pebblepost/refs/heads/main/security/pebblepost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketing
- Advertising
- Direct Mail
- Connected TV
- Retail
- Commerce
- Identity
- Analytics
---

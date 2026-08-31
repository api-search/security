---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vungle.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liftoff.io
  spf: true
hosts:
- cert_expires: Sep 26 11:56:32 2026 GMT
  host: vungle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 02:36:02 2026 GMT
  host: docs.liftoff.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 02:36:02 2026 GMT
  host: data.liftoff.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vungle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vungle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vungle
provider_slug: vungle
slug: vungle-domain-security
source_filename: vungle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vungle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:56:32 2026 GMT\n  hsts: false\n- host: docs.liftoff.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:36:02 2026 GMT\n  hsts: false\n- host: data.liftoff.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:36:02 2026 GMT\n  hsts: null\ndomains:\n- domain: vungle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: liftoff.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vungle/refs/heads/main/security/vungle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Mobile
- Monetization
- User Acquisition
- Ad Tech
- Analytics
- Reporting
---

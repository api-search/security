---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stashaway.sg
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stashaway.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stashaway.my
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stashaway.ae
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stashaway.hk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stashaway.co.th
  spf: true
hosts:
- cert_expires: Nov 15 07:31:35 2026 GMT
  host: www.stashaway.sg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: www.stashaway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 17:24:39 2026 GMT
  host: www.stashaway.my
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 07:56:12 2026 GMT
  host: www.stashaway.ae
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 06:33:36 2026 GMT
  host: www.stashaway.hk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 18:21:22 2026 GMT
  host: www.stashaway.co.th
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: app.stashaway.sg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.stashaway.sg
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 01:30:01 2026 GMT
  host: vdp.stashaway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stashaway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StashAway, probed live across 9 host(s) and 6 registrable domain(s). 9 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StashAway
provider_slug: stashaway
slug: stashaway-domain-security
source_filename: stashaway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every StashAway regional website host, the mobile-app\n  API host (api.stashaway.sg) and the vulnerability-disclosure host (vdp.stashaway.com)\nhosts:\n- host: www.stashaway.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 07:31:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.stashaway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\n- host: www.stashaway.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 17:24:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.stashaway.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 07:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.stashaway.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:33:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.stashaway.co.th\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Nov  7 18:21:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.stashaway.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.stashaway.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: vdp.stashaway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 01:30:01 2026 GMT\n  hsts: null\ndomains:\n- domain: stashaway.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stashaway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stashaway.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stashaway.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stashaway.hk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n- domain: stashaway.co.th\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stashaway/refs/heads/main/security/stashaway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wealth Management
- Investing
- Robo-Advisor
- Financial Services
- Asset Management
- ETFs
- Cash Management
- Fintech
- Singapore
- Private Markets
---

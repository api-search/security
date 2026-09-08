---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: essendant.com
  spf: true
hosts:
- cert_expires: Nov  7 06:52:02 2026 GMT
  host: www.essendant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: sso.essendant.com
  hsts: false
  https: true
  note: AD FS identity host serving the OpenID Connect discovery document; negotiates TLS 1.2, not 1.3.
  tls_version: TLSv1.2
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: login.essendant.com
  hsts: false
  https: true
  note: Second AD FS identity host; same posture as sso.
  tls_version: TLSv1.2
- cert_expires: Nov 17 22:21:02 2026 GMT
  host: info.essendant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Campaign/landing host (ECDB documentation pages). The only Essendant host observed sending HSTS.
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Essendant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Essendant, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Essendant
provider_slug: essendant
slug: essendant-domain-security
source_filename: essendant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of the apis.yml hosts plus the identity and campaign hosts found\n  during contract discovery (sso.essendant.com, login.essendant.com, info.essendant.com)\nhosts:\n- host: www.essendant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 06:52:02 2026 GMT\n  hsts: false\n- host: sso.essendant.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n  note: AD FS identity host serving the OpenID Connect discovery document; negotiates TLS 1.2, not 1.3.\n- host: login.essendant.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n  note: Second AD FS identity host; same posture as sso.\n- host: info.essendant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 22:21:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    Campaign/landing host (ECDB documentation pages).\
  \ The only Essendant host observed\n    sending HSTS.\ndomains:\n- domain: essendant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- No HSTS on the primary web host or on either identity host; only the campaign host sends it.\n- Both AD FS identity hosts terminate at TLS 1.2 while the marketing estate is on TLS 1.3.\n- No CAA records and no DNSSEC on essendant.com.\n- DMARC is published but the policy is p=none, so nothing is enforced against spoofed mail.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/essendant/refs/heads/main/security/essendant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wholesale
- Distribution
- Supply Chain
- Office Supplies
- Fulfillment
- 3PL
- B2B
- EDI
- Ecommerce
- JanSan
- Foodservice
---

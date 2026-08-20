---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: games24x7.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rummycircle.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: my11circle.com
  spf: true
hosts:
- cert_expires: Oct  3 22:27:01 2026 GMT
  host: www.games24x7.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.rummycircle.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.my11circle.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Games24X7 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Games24x7, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Games24x7
provider_slug: games24x7
slug: games24x7-domain-security
source_filename: games24x7-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the two consumer brand hosts\n  (rummycircle.com, my11circle.com) Games24x7 operates\nnote: >-\n  Games24x7 publishes no API host, so there is no API-host row here. The corporate\n  site and the two consumer product hosts were probed instead. No CAA record and no\n  DNSSEC on any of the three registrable domains; HSTS is served on the corporate\n  Webflow site but not on either product host.\nhosts:\n- host: www.games24x7.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:27:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.rummycircle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: www.my11circle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: false\n  hsts_max_age: null\ndomains:\n- domain: games24x7.com\n  dnssec: false\n\
  \  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rummycircle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: my11circle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/games24x7/refs/heads/main/security/games24x7-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Online Gaming
- Skill Gaming
- Fantasy Sports
- Real-Money Gaming
- Consumer Applications
- Entertainment
- Mobile Games
- India
---

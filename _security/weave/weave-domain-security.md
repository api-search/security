---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getweave.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: weaveconnect.com
  spf: false
hosts:
- cert_expires: Oct 13 17:27:14 2026 GMT
  host: www.getweave.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:12:01 2026 GMT
  host: dp.getweave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 00:05:58 2026 GMT
  host: api.weaveconnect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weave, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weave
provider_slug: weave
slug: weave-domain-security
source_filename: weave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:27:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dp.getweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weaveconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 00:05:58 2026 GMT\n  hsts: null\ndomains:\n- domain: getweave.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: weaveconnect.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/security/weave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Communication
- Messaging
- Payments
- Healthcare
- VoIP
- Telephony
- Reviews
- Scheduling
- SMB
- Developer Platform
- OAuth
---

---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boardeffect.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "amazonaws.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: diligent.com
  spf: true
hosts:
- cert_expires: Sep 13 02:03:52 2026 GMT
  host: www.boardeffect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:13:49 2026 GMT
  host: www.diligent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boardeffect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoardEffect, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BoardEffect
provider_slug: boardeffect
slug: boardeffect-domain-security
source_filename: boardeffect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boardeffect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:03:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.diligent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boardeffect.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: diligent.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boardeffect/refs/heads/main/security/boardeffect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Board Management
- Board Portal
- Governance
- Meetings
- Nonprofit
- Diligent
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: personifycorp.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:abuse@wildapricot.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wildapricot.com
  spf: true
hosts:
- cert_expires: Sep 24 04:02:47 2026 GMT
  host: personifycorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 02:04:26 2026 GMT
  host: gethelp.wildapricot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:53:34 2026 GMT
  host: api.wildapricot.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Personifycorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Personify, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Personify
provider_slug: personifycorp
slug: personifycorp-domain-security
source_filename: personifycorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: personifycorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:02:47 2026 GMT\n  hsts: false\n- host: gethelp.wildapricot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:04:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wildapricot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:53:34 2026 GMT\n  hsts: null\ndomains:\n- domain: personifycorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wildapricot.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:abuse@wildapricot.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/personifycorp/refs/heads/main/security/personifycorp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Association Management
- AMS
- Membership
- Nonprofit
- Events
- Constituent Management
- CRM
---

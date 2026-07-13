---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailgun.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nylas.com
  spf: true
hosts:
- cert_expires: Aug 25 07:03:07 2026 GMT
  host: www.mailgun.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 01:33:30 2026 GMT
  host: www.nylas.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inbox, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Inbox
provider_slug: inbox
slug: inbox-domain-security
source_filename: inbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailgun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 07:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.nylas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 01:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mailgun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nylas.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inbox/refs/heads/main/security/inbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Inbox
- Messaging
- Deliverability
- Transactional Email
---

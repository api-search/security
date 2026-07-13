---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: people.inc
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iac.com
  spf: true
hosts:
- cert_expires: Aug 18 13:14:14 2026 GMT
  host: www.people.inc
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 15:03:00 2026 GMT
  host: www.iac.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 17:30:27 2026 GMT
  host: people.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meredith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dotdash Meredith / People Inc, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dotdash Meredith / People Inc
provider_slug: meredith
slug: meredith-domain-security
source_filename: meredith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.people.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:14:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.iac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:03:00 2026 GMT\n  hsts: null\n- host: people.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: people.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: iac.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meredith/refs/heads/main/security/meredith-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- Publishing
- Magazines
- Content
- Advertising
- Contextual Advertising
- Lifestyle
- News
- RSS
- Sitemaps
- Robots
- AI Policy
- IAC
---

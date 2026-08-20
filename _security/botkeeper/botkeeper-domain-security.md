---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: botkeeper.com
  spf: true
hosts:
- cert_expires: Sep 19 22:14:13 2026 GMT
  host: www.botkeeper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 14:23:08 2026 GMT
  host: status.botkeeper.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: ipa.botkeeper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Botkeeper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Botkeeper, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Botkeeper
provider_slug: botkeeper
slug: botkeeper-domain-security
source_filename: botkeeper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.botkeeper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:14:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.botkeeper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 14:23:08 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: ipa.botkeeper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: botkeeper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botkeeper/refs/heads/main/security/botkeeper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Accounting
- Bookkeeping
- Financial-Services
- Artificial Intelligence
- Automation
- Software-as-a-Service
- Banking Data
- Practice Management
- Small Business
---

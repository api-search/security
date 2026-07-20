---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: caplinked.com
  spf: true
hosts:
- cert_expires: Aug 20 15:13:47 2026 GMT
  host: caplinked.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 08:10:25 2026 GMT
  host: developer.caplinked.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: sandbox.caplinked.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Caplinked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caplinked, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Caplinked
provider_slug: caplinked
slug: caplinked-domain-security
source_filename: caplinked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caplinked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:13:47 2026 GMT\n  hsts: false\n- host: developer.caplinked.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 08:10:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandbox.caplinked.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: caplinked.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caplinked/refs/heads/main/security/caplinked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Virtual Data Room
- Document Security
- File Sharing
- Due Diligence
- Mergers and Acquisitions
- Digital Rights Management
- Compliance
- Data Room
- Security
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wuzzuf.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: basharsoft.com
  spf: true
hosts:
- cert_expires: Oct 11 16:15:01 2026 GMT
  host: wuzzuf.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 17:07:17 2026 GMT
  host: basharsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wuzzuf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wuzzuf, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wuzzuf
provider_slug: wuzzuf
slug: wuzzuf-domain-security
source_filename: wuzzuf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wuzzuf.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 16:15:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: basharsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 17:07:17 2026 GMT\n  hsts: false\ndomains:\n- domain: wuzzuf.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: basharsoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wuzzuf/refs/heads/main/security/wuzzuf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Jobs
- Recruitment
- Careers
- Employment
- HR
- Egypt
---

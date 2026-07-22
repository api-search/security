---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zmanda.com
  spf: true
hosts:
- cert_expires: Sep 22 20:58:44 2026 GMT
  host: www.zmanda.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zmanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zmanda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zmanda
provider_slug: zmanda
slug: zmanda-domain-security
source_filename: zmanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zmanda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zmanda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zmanda/refs/heads/main/security/zmanda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Backup
- Recovery
- Data Protection
- Disaster Recovery
- Cloud Backup
- Storage
- Enterprise Software
- Amanda
- Database Backup
---

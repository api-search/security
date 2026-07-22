---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zerto.com
  spf: false
hosts:
- cert_expires: Sep 22 14:29:11 2026 GMT
  host: www.zerto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zerto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zerto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Zerto
provider_slug: zerto
slug: zerto-domain-security
source_filename: zerto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zerto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:29:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zerto.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerto/refs/heads/main/security/zerto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Disaster Recovery
- Data Protection
- Backup
- Ransomware Resilience
- Business Continuity
- Cloud Migration
- Replication
- Infrastructure
---

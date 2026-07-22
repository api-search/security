---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloudlock.com
  spf: true
hosts:
- cert_expires: Sep  5 03:14:30 2026 GMT
  host: www.cloudlock.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudlock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudLock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CloudLock
provider_slug: cloudlock
slug: cloudlock-domain-security
source_filename: cloudlock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudlock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:14:30 2026 GMT\n  hsts: false\ndomains:\n- domain: cloudlock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudlock/refs/heads/main/security/cloudlock-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Security
- CASB
- Cloud Access Security Broker
- Data Loss Prevention
- Cloud Security
- SaaS Security
- Cisco
---

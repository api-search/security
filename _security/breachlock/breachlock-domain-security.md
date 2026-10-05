---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: breachlock.com
  spf: true
hosts:
- cert_expires: Dec  2 18:21:07 2026 GMT
  host: www.breachlock.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Breachlock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BreachLock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BreachLock
provider_slug: breachlock
slug: breachlock-domain-security
source_filename: breachlock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breachlock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 18:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: breachlock.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breachlock/refs/heads/main/security/breachlock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Penetration Testing
- Attack Surface Management
- Red Team
- Software-as-a-Service
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloverleaf.me
  spf: true
hosts:
- cert_expires: Nov 27 18:38:44 2026 GMT
  host: cloverleaf.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloverleafme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloverleafme, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloverleafme
provider_slug: cloverleafme
slug: cloverleafme-domain-security
source_filename: cloverleafme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloverleaf.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 18:38:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloverleaf.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloverleafme/refs/heads/main/security/cloverleafme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Team Performance
- AI Coaching
- Behavioral Assessment
- Workplace Integration
- Leadership Development
- Company
---

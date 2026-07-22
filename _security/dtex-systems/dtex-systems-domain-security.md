---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dtexsystems.com
  spf: true
hosts:
- cert_expires: Aug 20 17:15:23 2026 GMT
  host: www.dtexsystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dtex Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dtex Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dtex Systems
provider_slug: dtex-systems
slug: dtex-systems-domain-security
source_filename: dtex-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dtexsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:15:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dtexsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dtex-systems/refs/heads/main/security/dtex-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Insider Risk Management
- Data Loss Prevention
- User Activity Monitoring
- Behavioral Intelligence
- Threat Detection
- Security
---

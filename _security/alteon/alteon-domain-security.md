---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: radware.com
  spf: true
hosts:
- cert_expires: Sep  5 09:17:13 2026 GMT
  host: radware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alteon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alteon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alteon
provider_slug: alteon
slug: alteon-domain-security
source_filename: alteon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: radware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 09:17:13 2026 GMT\n  hsts: false\ndomains:\n- domain: radware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alteon/refs/heads/main/security/alteon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure
- Application Delivery
- Load Balancing
- Application Delivery Controller
- Application Security
- Networking
- Radware
---

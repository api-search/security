---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sava.health
  spf: true
hosts:
- cert_expires: Sep  1 19:43:00 2026 GMT
  host: www.sava.health
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sava Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAVA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SAVA
provider_slug: sava
slug: sava-domain-security
source_filename: sava-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sava.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:43:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: sava.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sava/refs/heads/main/security/sava-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Digital Health
- Biosensor
- Wearables
- Continuous Monitoring
- Preventative Health
- HealthTech
- MCP
---

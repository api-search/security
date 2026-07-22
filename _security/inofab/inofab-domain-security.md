---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inofab.health
  spf: true
hosts:
- cert_expires: Oct  7 15:00:00 2026 GMT
  host: www.inofab.health
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inofab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inofab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inofab
provider_slug: inofab
slug: inofab-domain-security
source_filename: inofab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inofab.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: inofab.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inofab/refs/heads/main/security/inofab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Health
- Respiratory
- Spirometry
- Medical Devices
- Remote Patient Monitoring
- Connected Devices
- Healthcare
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sprinterhealth.com
  spf: true
hosts:
- cert_expires: Sep 29 14:47:50 2026 GMT
  host: www.sprinterhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sprinter Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sprinter Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sprinter Health
provider_slug: sprinter-health
slug: sprinter-health-domain-security
source_filename: sprinter-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sprinterhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:47:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sprinterhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprinter-health/refs/heads/main/security/sprinter-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- In-Home Care
- Preventive Care
- Diagnostics
- Telehealth
- Care Navigation
---

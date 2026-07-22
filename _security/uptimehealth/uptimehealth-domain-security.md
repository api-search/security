---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uptimehealth.com
  spf: true
hosts:
- cert_expires: Oct 16 00:03:37 2026 GMT
  host: uptimehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Uptimehealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UptimeHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UptimeHealth
provider_slug: uptimehealth
slug: uptimehealth-domain-security
source_filename: uptimehealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uptimehealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 00:03:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uptimehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptimehealth/refs/heads/main/security/uptimehealth-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Healthcare
- Dental
- Medical Equipment
- Compliance
- Facilities Management
- Equipment Maintenance
---

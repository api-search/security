---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brighthealthplan.com
  spf: true
hosts:
- cert_expires: Oct  6 23:05:09 2026 GMT
  host: www.brighthealthplan.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bright Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bright Health
provider_slug: bright-health
slug: bright-health-domain-security
source_filename: bright-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brighthealthplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:05:09 2026 GMT\n  hsts: null\ndomains:\n- domain: brighthealthplan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-health/refs/heads/main/security/bright-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthtech
- Health Insurance
- Insurance
- Medicare Advantage
- ACA
- Value-Based Care
- Defunct Brand
---

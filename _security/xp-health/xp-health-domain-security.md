---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xphealth.co
  spf: true
hosts:
- cert_expires: Dec  8 18:49:43 2026 GMT
  host: xphealth.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xp Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XP Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: XP Health
provider_slug: xp-health
slug: xp-health-domain-security
source_filename: xp-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xphealth.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 18:49:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xphealth.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xp-health/refs/heads/main/security/xp-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthtech
- Vision Benefits
- Employee Benefits
- Eyewear
- Vision Care
- Insurance
---

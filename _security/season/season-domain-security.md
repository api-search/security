---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seasonhealth.com
  spf: true
hosts:
- cert_expires: Aug 20 15:03:13 2026 GMT
  host: www.seasonhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Season Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Season Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Season Health
provider_slug: season
slug: season-domain-security
source_filename: season-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seasonhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:03:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seasonhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/season/refs/heads/main/security/season-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Nutrition
- Food as Medicine
- Digital Health
- Chronic Care
- Telehealth
---

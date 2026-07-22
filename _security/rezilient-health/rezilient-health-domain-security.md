---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rezilienthealth.com
  spf: true
hosts:
- cert_expires: Sep  9 15:34:08 2026 GMT
  host: rezilienthealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rezilient Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rezilient Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rezilient Health
provider_slug: rezilient-health
slug: rezilient-health-domain-security
source_filename: rezilient-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rezilienthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 15:34:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rezilienthealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rezilient-health/refs/heads/main/security/rezilient-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Primary Care
- Telehealth
- Employer Benefits
- Hybrid Care
---

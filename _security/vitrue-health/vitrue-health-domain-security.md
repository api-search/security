---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vitruehealth.com
  spf: true
hosts:
- cert_expires: Aug 28 05:58:49 2026 GMT
  host: vitruehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vitrue Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vitrue Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vitrue Health
provider_slug: vitrue-health
slug: vitrue-health-domain-security
source_filename: vitrue-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vitruehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 05:58:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vitruehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitrue-health/refs/heads/main/security/vitrue-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Health
- Musculoskeletal
- Ergonomics
- Workplace Wellness
- DSE Compliance
- Occupational Health
- Artificial Intelligence
---

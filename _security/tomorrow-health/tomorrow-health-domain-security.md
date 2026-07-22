---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tomorrowhealth.com
  spf: true
hosts:
- cert_expires: Aug 25 15:12:01 2026 GMT
  host: tomorrowhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tomorrow Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tomorrow Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tomorrow Health
provider_slug: tomorrow-health
slug: tomorrow-health-domain-security
source_filename: tomorrow-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tomorrowhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tomorrowhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomorrow-health/refs/heads/main/security/tomorrow-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Home Health
- DMEPOS
- Durable Medical Equipment
- Health Tech
- Care Coordination
- Health Insurance
---

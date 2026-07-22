---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pearlhealth.com
  spf: true
hosts:
- cert_expires: Sep 13 14:02:27 2026 GMT
  host: pearlhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pearl Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pearl Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pearl Health
provider_slug: pearl-health
slug: pearl-health-domain-security
source_filename: pearl-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pearlhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pearlhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pearl-health/refs/heads/main/security/pearl-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Value-Based Care
- Medicare
- Health Systems
- Primary Care
- Population Health
- Health Analytics
---

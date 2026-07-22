---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unohealth.com
  spf: false
hosts:
- cert_expires: Sep 24 12:18:13 2026 GMT
  host: www.unohealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uno Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uno Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Uno Health
provider_slug: uno-health
slug: uno-health-domain-security
source_filename: uno-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:18:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unohealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uno-health/refs/heads/main/security/uno-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medicare
- Benefits
- Enrollment
- Health Plans
- Government Programs
---

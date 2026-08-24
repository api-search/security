---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greatergoodhealth.com
  spf: true
hosts:
- cert_expires: Nov  4 17:00:03 2026 GMT
  host: greatergoodhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greater Good Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greater Good Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Greater Good Health
provider_slug: greater-good-health
slug: greater-good-health-domain-security
source_filename: greater-good-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greatergoodhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 17:00:03 2026 GMT\n  hsts: false\ndomains:\n- domain: greatergoodhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greater-good-health/refs/heads/main/security/greater-good-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Senior Care
- Value-Based Care
- Medicare
- Nurse Practitioners
- Clinics
- Population Health
- Health Services
---

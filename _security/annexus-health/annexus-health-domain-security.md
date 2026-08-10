---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: annexushealth.com
  spf: true
hosts:
- cert_expires: Sep 14 10:03:01 2026 GMT
  host: www.annexushealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 21:06:35 2026 GMT
  host: login.live.annexushealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Annexus Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Annexus Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Annexus Health
provider_slug: annexus-health
slug: annexus-health-domain-security
source_filename: annexus-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.annexushealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:03:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: login.live.annexushealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:06:35 2026 GMT\n  hsts: null\ndomains:\n- domain: annexushealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/annexus-health/refs/heads/main/security/annexus-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Technology
- Patient Access
- Financial Assistance
- Oncology
- Revenue Cycle
- Copay Assistance
- Identity
- OpenID Connect
- HITRUST
---

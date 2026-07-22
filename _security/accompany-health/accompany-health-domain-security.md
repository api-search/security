---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: accompanyhealth.com
  spf: true
hosts:
- cert_expires: Oct 10 06:24:42 2026 GMT
  host: www.accompanyhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accompany Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accompany Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Accompany Health
provider_slug: accompany-health
slug: accompany-health-domain-security
source_filename: accompany-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accompanyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:24:42 2026 GMT\n  hsts: null\ndomains:\n- domain: accompanyhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accompany-health/refs/heads/main/security/accompany-health-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Home Health
- Telehealth
- Behavioral Health
- Value-Based Care
- Medicaid
- Medicare
- HIPAA
---

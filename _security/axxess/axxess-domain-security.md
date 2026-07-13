---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: axxess.com
  spf: true
hosts:
- cert_expires: Nov 14 15:21:53 2026 GMT
  host: www.axxess.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 10:39:38 2026 GMT
  host: engage.axxess.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axxess Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axxess, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Axxess
provider_slug: axxess
slug: axxess-domain-security
source_filename: axxess-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axxess.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 14 15:21:53 2026 GMT\n  hsts: false\n- host: engage.axxess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:39:38 2026 GMT\n  hsts: false\ndomains:\n- domain: axxess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axxess/refs/heads/main/security/axxess-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Home Health
- Hospice
- Private Duty
- EHR
- Healthcare
- FHIR
- OASIS
- Billing
- Scheduling
- Visit Documentation
---

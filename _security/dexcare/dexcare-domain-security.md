---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dexcare.com
  spf: true
hosts:
- cert_expires: Sep 24 13:01:15 2026 GMT
  host: dexcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dexcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DexCare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DexCare
provider_slug: dexcare
slug: dexcare-domain-security
source_filename: dexcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dexcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:01:15 2026 GMT\n  hsts: false\ndomains:\n- domain: dexcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/security/dexcare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health IT
- Patient Access
- Scheduling
- Virtual Care
- Telehealth
- Care Navigation
- Provider Data
- SDK
---

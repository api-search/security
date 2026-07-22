---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aspenrxhealth.com
  spf: true
hosts:
- cert_expires: Sep 21 00:36:52 2026 GMT
  host: aspenrxhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aspen Rxhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aspen RxHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aspen RxHealth
provider_slug: aspen-rxhealth
slug: aspen-rxhealth-domain-security
source_filename: aspen-rxhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aspenrxhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:36:52 2026 GMT\n  hsts: false\ndomains:\n- domain: aspenrxhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspen-rxhealth/refs/heads/main/security/aspen-rxhealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Pharmacy
- Medication Therapy Management
- Clinical Pharmacists
- Medication Adherence
- Digital Health
- Telehealth
---

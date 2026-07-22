---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: glooko.com
  spf: true
hosts:
- cert_expires: Sep 13 08:01:16 2026 GMT
  host: glooko.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glooko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glooko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Glooko
provider_slug: glooko
slug: glooko-domain-security
source_filename: glooko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glooko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:01:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: glooko.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glooko/refs/heads/main/security/glooko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Diabetes
- Diabetes Management
- Healthcare
- Digital Health
- Remote Patient Monitoring
- Medical Devices
- EHR Integration
- FHIR
- Interoperability
- Chronic Care
- Life Sciences
---

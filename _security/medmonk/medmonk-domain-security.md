---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medmonk.com
  spf: true
hosts:
- cert_expires: Sep 24 04:11:27 2026 GMT
  host: medmonk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medmonk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medmonk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Medmonk
provider_slug: medmonk
slug: medmonk-domain-security
source_filename: medmonk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medmonk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:11:27 2026 GMT\n  hsts: false\ndomains:\n- domain: medmonk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medmonk/refs/heads/main/security/medmonk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Pharma Market Access
- FHIR
- Medication Adherence
- Copay Assistance
- Prior Authorization
- Interoperability
- HIPAA
---

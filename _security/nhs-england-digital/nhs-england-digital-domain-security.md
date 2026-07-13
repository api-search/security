---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhs.uk
  spf: true
hosts:
- cert_expires: Sep 24 21:58:44 2026 GMT
  host: digital.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nhs England Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NHS England Digital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NHS England Digital
provider_slug: nhs-england-digital
slug: nhs-england-digital-domain-security
source_filename: nhs-england-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digital.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:44 2026 GMT\n  hsts: null\ndomains:\n- domain: nhs.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-england-digital/refs/heads/main/security/nhs-england-digital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Clinical
- Demographics
- FHIR
- Government
- Health
- Healthcare
- NHS
- Open Data
- Patient Records
- Prescriptions
- UK
---

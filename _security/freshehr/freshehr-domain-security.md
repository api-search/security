---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freshehr.com
  spf: true
hosts:
- cert_expires: Nov 20 06:27:22 2026 GMT
  host: freshehr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshehr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for freshEHR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: freshEHR
provider_slug: freshehr
slug: freshehr-domain-security
source_filename: freshehr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freshehr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 06:27:22 2026 GMT\n  hsts: false\ndomains:\n- domain: freshehr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshehr/refs/heads/main/security/freshehr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consulting
- Health
- Healthcare
- Clinical Informatics
- Electronic Health Records
- openEHR
- HL7 FHIR
- SNOMED CT
- Interoperability
- Standards
- Training
- United Kingdom
---

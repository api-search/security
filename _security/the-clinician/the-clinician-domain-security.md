---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: theclinician.com
  spf: true
hosts:
- cert_expires: Oct 17 01:53:47 2026 GMT
  host: theclinician.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Clinician Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Clinician, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Clinician
provider_slug: the-clinician
slug: the-clinician-domain-security
source_filename: the-clinician-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theclinician.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 01:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theclinician.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-clinician/refs/heads/main/security/the-clinician-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health IT
- Patient Reported Outcomes
- PROMs
- Value-Based Care
- Clinical Data
- Interoperability
- FHIR
- openEHR
- Digital Health
- New Zealand
---

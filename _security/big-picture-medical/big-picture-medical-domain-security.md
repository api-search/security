---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bigpicturemedical.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.bigpicturemedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Big Picture Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Big Picture Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Big Picture Medical
provider_slug: big-picture-medical
slug: big-picture-medical-domain-security
source_filename: big-picture-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bigpicturemedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bigpicturemedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-picture-medical/refs/heads/main/security/big-picture-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health Care
- Electronic Health Records
- openEHR
- FHIR
- HL7
- Interoperability
- Clinical Data
- Care Pathways
- Workflow
- Orchestration
- No Code
- NHS
- United Kingdom
---

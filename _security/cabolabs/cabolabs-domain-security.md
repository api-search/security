---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cabolabs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: atomik.app
  spf: true
hosts:
- cert_expires: Nov 29 15:57:54 2026 GMT
  host: cabolabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 15:57:46 2026 GMT
  host: atomik.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cabolabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CaboLabs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CaboLabs
provider_slug: cabolabs
slug: cabolabs-domain-security
source_filename: cabolabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cabolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 15:57:54 2026 GMT\n  hsts: false\n- host: atomik.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 15:57:46 2026 GMT\n  hsts: false\ndomains:\n- domain: cabolabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: atomik.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cabolabs/refs/heads/main/security/cabolabs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Interoperability
- openEHR
- FHIR
- HL7
- Clinical Data Repository
- Electronic Health Records
- Standards
- SNOMED CT
- DICOM
- Medical Records
- Uruguay
---

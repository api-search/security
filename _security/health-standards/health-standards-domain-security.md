---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "symantec.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hl7.org
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.hl7.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Health Standards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Health Standards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Health Standards
provider_slug: health-standards
slug: health-standards-domain-security
source_filename: health-standards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hl7.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hl7.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"symantec.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-standards/refs/heads/main/security/health-standards-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CDA
- DICOM
- FHIR
- Health Standards
- Healthcare Interoperability
- HL7
- ICD
- LOINC
- SNOMED CT
- US Core
---

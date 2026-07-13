---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 iodef "mailto:dadm@sectra.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sectra.com
  spf: true
hosts:
- cert_expires: Apr  5 09:26:43 2027 GMT
  host: sectra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 09:26:43 2027 GMT
  host: medical.sectra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 09:26:43 2027 GMT
  host: amplifiermarketplace.sectra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sectra Imaging Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sectra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sectra
provider_slug: sectra-imaging
slug: sectra-imaging-domain-security
source_filename: sectra-imaging-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sectra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 09:26:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: medical.sectra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 09:26:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: amplifiermarketplace.sectra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 09:26:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sectra.com\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 iodef \"mailto:dadm@sectra.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sectra-imaging/refs/heads/main/security/sectra-imaging-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Medical Imaging
- Enterprise Imaging
- PACS
- VNA
- Radiology
- Pathology
- Healthcare
- DICOM
- DICOMweb
- HL7
- FHIR
- FHIRcast
- IHE XDS
- Interoperability
- Partner API
---

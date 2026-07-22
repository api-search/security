---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sironamedical.com
  spf: true
hosts:
- cert_expires: Oct 12 21:13:34 2026 GMT
  host: sironamedical.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sirona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sirona Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sirona Medical
provider_slug: sirona
slug: sirona-domain-security
source_filename: sirona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sironamedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:13:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sironamedical.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirona/refs/heads/main/security/sirona-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Imaging
- Radiology
- PACS
- DICOM
- HL7
- FHIR
- Cloud
- Artificial Intelligence
- Health IT
---

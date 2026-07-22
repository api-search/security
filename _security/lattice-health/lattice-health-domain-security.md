---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: latticehealthai.com
  spf: true
hosts:
- cert_expires: Sep  5 17:04:25 2026 GMT
  host: www.latticehealthai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lattice Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lattice Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lattice Health
provider_slug: lattice-health
slug: lattice-health-domain-security
source_filename: lattice-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.latticehealthai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:04:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: latticehealthai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lattice-health/refs/heads/main/security/lattice-health-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Health IT
- Artificial Intelligence
- AI Governance
- Clinical AI
- Medical Imaging
- Radiology
- DICOM
- HL7
- Compliance
- Monitoring
- Observability
---

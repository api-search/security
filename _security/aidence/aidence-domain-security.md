---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aidence.com
  spf: true
hosts:
- cert_expires: Sep  2 09:10:42 2026 GMT
  host: aidence.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aidence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aidence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aidence
provider_slug: aidence
slug: aidence-domain-security
source_filename: aidence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aidence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:10:42 2026 GMT\n  hsts: false\ndomains:\n- domain: aidence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidence/refs/heads/main/security/aidence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Radiology
- Medical Imaging
- Lung Cancer Screening
- Clinical Decision Support
- DICOM
---

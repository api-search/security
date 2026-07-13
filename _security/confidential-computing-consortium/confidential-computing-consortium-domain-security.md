---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: confidentialcomputing.io
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: confidentialcomputing.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confidential Computing Consortium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confidential Computing Consortium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Confidential Computing Consortium
provider_slug: confidential-computing-consortium
slug: confidential-computing-consortium-domain-security
source_filename: confidential-computing-consortium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: confidentialcomputing.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: confidentialcomputing.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confidential-computing-consortium/refs/heads/main/security/confidential-computing-consortium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Attestation
- Confidential Computing
- Hardware
- Linux Foundation
- Open Source
- Privacy
- Security
- TEE
- Trusted Execution Environment
---

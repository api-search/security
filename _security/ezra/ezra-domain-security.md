---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ezra.com
  spf: true
hosts:
- cert_expires: Oct  1 10:34:07 2026 GMT
  host: ezra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ezra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ezra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ezra
provider_slug: ezra
slug: ezra-domain-security
source_filename: ezra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ezra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:34:07 2026 GMT\n  hsts: false\ndomains:\n- domain: ezra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezra/refs/heads/main/security/ezra-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Imaging
- Preventive Health
- Cancer Screening
- MRI
- Diagnostics
---

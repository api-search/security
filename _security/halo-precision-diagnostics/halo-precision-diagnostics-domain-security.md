---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: halodx.com
  spf: true
hosts:
- cert_expires: Nov 11 00:24:31 2026 GMT
  host: www.halodx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Halo Precision Diagnostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HALO Precision Diagnostics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HALO Precision Diagnostics
provider_slug: halo-precision-diagnostics
slug: halo-precision-diagnostics-domain-security
source_filename: halo-precision-diagnostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.halodx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 00:24:31 2026 GMT\n  hsts: false\ndomains:\n- domain: halodx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halo-precision-diagnostics/refs/heads/main/security/halo-precision-diagnostics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Diagnostics
- Medical Imaging
- Radiology
- Cancer
- Precision Medicine
- Genomics
- Early Detection
- Artificial Intelligence
---

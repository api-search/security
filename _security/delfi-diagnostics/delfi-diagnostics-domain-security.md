---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: delfidiagnostics.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: delfidiagnostics.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Delfi Diagnostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delfi Diagnostics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Delfi Diagnostics
provider_slug: delfi-diagnostics
slug: delfi-diagnostics-domain-security
source_filename: delfi-diagnostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delfidiagnostics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: delfidiagnostics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delfi-diagnostics/refs/heads/main/security/delfi-diagnostics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Diagnostics
- Precision Oncology
- Liquid Biopsy
- Cancer Screening
- Genomics
- Machine Learning
- Healthcare
---

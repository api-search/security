---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rescale.com
  spf: true
hosts:
- cert_expires: Sep  8 16:52:17 2026 GMT
  host: rescale.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 16:36:33 2026 GMT
  host: platform.rescale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: htc.rescale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rescale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rescale, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Rescale
provider_slug: rescale
slug: rescale-domain-security
source_filename: rescale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rescale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 16:52:17 2026 GMT\n  hsts: false\n- host: platform.rescale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:36:33 2026 GMT\n  hsts: null\n- host: htc.rescale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rescale.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rescale/refs/heads/main/security/rescale-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- High Performance Computing
- Simulation
- Cloud
- Engineering
- CAE
- HPC
- AI Physics
- Jobs
- Compute
---

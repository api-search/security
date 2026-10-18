---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brighturo.com
  spf: true
hosts:
- cert_expires: Nov 30 10:04:18 2026 GMT
  host: brighturo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bright Uro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Uro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bright Uro
provider_slug: bright-uro
slug: bright-uro-domain-security
source_filename: bright-uro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brighturo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 10:04:18 2026 GMT\n  hsts: false\ndomains:\n- domain: brighturo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-uro/refs/heads/main/security/bright-uro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health Tech
- Medical Devices
- Diagnostics
- Urology
---

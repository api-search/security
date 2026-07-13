---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: r1rcm.com
  spf: true
hosts:
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: www.r1rcm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.r1rcm.com
  https: false
- host: api.r1rcm.com
  https: false
kind: domain-security
layout: security
method: probed
name: R1 Rcm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for R1 RCM, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: R1 RCM
provider_slug: r1-rcm
slug: r1-rcm-domain-security
source_filename: r1-rcm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.r1rcm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.r1rcm.com\n  https: false\n- host: api.r1rcm.com\n  https: false\ndomains:\n- domain: r1rcm.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/r1-rcm/refs/heads/main/security/r1-rcm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Revenue Cycle
- Technology
---

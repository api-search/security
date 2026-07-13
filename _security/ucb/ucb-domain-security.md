---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: berkeley.edu
  spf: true
hosts:
- cert_expires: Sep 14 20:03:09 2026 GMT
  host: www.berkeley.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: developers.api.berkeley.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 20:14:07 2026 GMT
  host: integration-services.berkeley.edu
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ucb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of California, Berkeley, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: University of California, Berkeley
provider_slug: ucb
slug: ucb-domain-security
source_filename: ucb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.berkeley.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:03:09 2026 GMT\n  hsts: false\n- host: developers.api.berkeley.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\n- host: integration-services.berkeley.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:14:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: berkeley.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucb/refs/heads/main/security/ucb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- United States
- California
---

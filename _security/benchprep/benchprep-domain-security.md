---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: benchprep.com
  spf: true
hosts:
- cert_expires: Nov 27 10:40:59 2026 GMT
  host: www.benchprep.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Benchprep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BenchPrep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BenchPrep
provider_slug: benchprep
slug: benchprep-domain-security
source_filename: benchprep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benchprep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 10:40:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: benchprep.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchprep/refs/heads/main/security/benchprep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- LMS
- Education
- Training
- SaaS
---

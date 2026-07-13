---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ksu.edu.sa
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: ksu.edu.sa
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: King Saud University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for King Saud University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: King Saud University
provider_slug: king-saud-university
slug: king-saud-university-domain-security
source_filename: king-saud-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ksu.edu.sa\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ksu.edu.sa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/security/king-saud-university-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Education
- Higher Education
- University
- Saudi Arabia
- Middle East
- Research
---

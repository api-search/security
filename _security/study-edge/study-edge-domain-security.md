---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: studyedge.com
  spf: true
hosts:
- cert_expires: Aug 31 12:58:42 2026 GMT
  host: www.studyedge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Study Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Study Edge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Study Edge
provider_slug: study-edge
slug: study-edge-domain-security
source_filename: study-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.studyedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 12:58:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: studyedge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/study-edge/refs/heads/main/security/study-edge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Online Learning
- Tutoring
- Test Preparation
- Math Education
- Students
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: synthace.com
  spf: true
hosts:
- cert_expires: Nov 17 23:17:00 2026 GMT
  host: www.synthace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synthace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Synthace
provider_slug: synthace
slug: synthace-domain-security
source_filename: synthace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synthace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:17:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synthace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthace/refs/heads/main/security/synthace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Life Sciences
- Biotechnology
- Laboratory Automation
- Design of Experiments
- Research and Development
- Scientific Data
- Cloud Platform
- Company
---

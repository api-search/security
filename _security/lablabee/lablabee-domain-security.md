---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lablabee.com
  spf: true
hosts:
- cert_expires: Sep 29 09:43:35 2026 GMT
  host: lablabee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lablabee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LabLabee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LabLabee
provider_slug: lablabee
slug: lablabee-domain-security
source_filename: lablabee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lablabee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:43:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lablabee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lablabee/refs/heads/main/security/lablabee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Telecommunications
- Network Automation
- Training
- Education
- Artificial Intelligence
- Cloud Native
- 5G
- Open RAN
- Kubernetes
- DevOps
- Sandboxes
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: noetik.ai
  spf: true
hosts:
- cert_expires: Sep 11 17:35:42 2026 GMT
  host: www.noetik.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noetik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noetik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Noetik
provider_slug: noetik
slug: noetik-domain-security
source_filename: noetik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noetik.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 17:35:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noetik.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noetik/refs/heads/main/security/noetik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Biotechnology
- Healthcare
- Oncology
- Foundation Models
- Spatial Biology
- Drug Discovery
- Life Sciences
---

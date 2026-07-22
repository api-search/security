---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: recursionpharma.com
  spf: true
hosts:
- cert_expires: Oct 11 20:38:30 2026 GMT
  host: recursionpharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recursion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recursion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Recursion
provider_slug: recursion
slug: recursion-domain-security
source_filename: recursion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recursionpharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 20:38:30 2026 GMT\n  hsts: false\ndomains:\n- domain: recursionpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recursion/refs/heads/main/security/recursion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Drug Discovery
- Artificial Intelligence
- Machine Learning
- Healthcare
---

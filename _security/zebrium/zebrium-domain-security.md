---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zebrium.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: www.zebrium.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zebrium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zebrium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zebrium
provider_slug: zebrium
slug: zebrium-domain-security
source_filename: zebrium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zebrium.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: zebrium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zebrium/refs/heads/main/security/zebrium-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Ai
- AIOps
- Machine Learning
- Log Management
- Observability
- Anomaly Detection
- Root Cause Analysis
- Acquired
---

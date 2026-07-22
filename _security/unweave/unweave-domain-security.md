---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unweave.io
  spf: true
hosts:
- cert_expires: Aug 24 10:44:50 2026 GMT
  host: www.unweave.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unweave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unweave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unweave
provider_slug: unweave
slug: unweave-domain-security
source_filename: unweave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unweave.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:44:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: unweave.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unweave/refs/heads/main/security/unweave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Machine Learning
- GPU Compute
- Developer Tools
- MLOps
- Cloud Infrastructure
- Serverless
- Development Environments
- Artificial Intelligence
---

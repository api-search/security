---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coreweave.com
  spf: true
hosts:
- cert_expires: Aug 22 07:19:12 2026 GMT
  host: www.coreweave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 02:23:17 2026 GMT
  host: cloud.coreweave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:19:06 2026 GMT
  host: docs.coreweave.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coreweave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreWeave, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CoreWeave
provider_slug: coreweave
slug: coreweave-domain-security
source_filename: coreweave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coreweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:19:12 2026 GMT\n  hsts: false\n- host: cloud.coreweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 02:23:17 2026 GMT\n  hsts: false\n- host: docs.coreweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:19:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coreweave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coreweave/refs/heads/main/security/coreweave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Cloud
- GPU
- HPC
- Inference
- Kubernetes
- Machine Learning
- Storage
---

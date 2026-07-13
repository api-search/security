---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: garden.io
  spf: true
hosts:
- cert_expires: Sep  1 11:53:44 2026 GMT
  host: garden.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 18:22:13 2026 GMT
  host: docs.garden.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: cloud.docs.garden.io
  https: false
kind: domain-security
layout: security
method: probed
name: Garden Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Garden, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Garden
provider_slug: garden-io
slug: garden-io-domain-security
source_filename: garden-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: garden.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:53:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.garden.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:22:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.docs.garden.io\n  https: false\ndomains:\n- domain: garden.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garden-io/refs/heads/main/security/garden-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kubernetes
- Developer Tools
- CI/CD
- Platform Engineering
- DevOps
- Preview Environments
---

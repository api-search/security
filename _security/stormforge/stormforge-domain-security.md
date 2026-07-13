---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stormforge.io
  spf: true
hosts:
- cert_expires: Sep 23 16:46:34 2026 GMT
  host: www.stormforge.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 08:33:47 2026 GMT
  host: docs.stormforge.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stormforge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StormForge, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StormForge
provider_slug: stormforge
slug: stormforge-domain-security
source_filename: stormforge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stormforge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:46:34 2026 GMT\n  hsts: false\n- host: docs.stormforge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stormforge.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stormforge/refs/heads/main/security/stormforge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Machine Learning
- Resource Management
- Rightsizing
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hydrahost.com
  spf: true
hosts:
- cert_expires: Oct  4 15:00:04 2026 GMT
  host: hydrahost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hydrahost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydrahost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hydrahost
provider_slug: hydrahost
slug: hydrahost-domain-security
source_filename: hydrahost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hydrahost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:00:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hydrahost.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydrahost/refs/heads/main/security/hydrahost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- GPU Cloud
- Bare Metal
- Artificial Intelligence
- Machine Learning
- Cloud Infrastructure
- Compute
- Neocloud
---

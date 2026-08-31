---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: armory.io
  spf: true
hosts:
- cert_expires: Oct 11 13:41:05 2026 GMT
  host: www.armory.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Armoryio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armory.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Armory.io
provider_slug: armoryio
slug: armoryio-domain-security
source_filename: armoryio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.armory.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:41:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: armory.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armoryio/refs/heads/main/security/armoryio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Devops
- Continuous Delivery
- Continuous Deployment
- Spinnaker
- Kubernetes
- Deployment
- GitOps
---

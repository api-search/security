---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rafay.co
  spf: true
hosts:
- cert_expires: Aug 28 02:10:59 2026 GMT
  host: docs.rafay.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rafay Product Documentation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rafay Product Documentation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rafay Product Documentation
provider_slug: rafay-product-documentation
slug: rafay-product-documentation-domain-security
source_filename: rafay-product-documentation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.rafay.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:10:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rafay.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rafay-product-documentation/refs/heads/main/security/rafay-product-documentation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kubernetes
- Cloud Native
- GPU
- AI
- Platform
---

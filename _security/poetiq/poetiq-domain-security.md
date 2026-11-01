---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: poetiq.ai
  spf: true
hosts:
- cert_expires: Dec 26 08:45:05 2026 GMT
  host: poetiq.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Poetiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poetiq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Poetiq
provider_slug: poetiq
slug: poetiq-domain-security
source_filename: poetiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poetiq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 08:45:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: poetiq.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/poetiq/security/poetiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Poetry
- Text Generation
---

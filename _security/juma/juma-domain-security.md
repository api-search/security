---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: juma.ai
  spf: true
hosts:
- cert_expires: Dec 10 01:02:22 2026 GMT
  host: juma.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Juma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Juma
provider_slug: juma
slug: juma-domain-security
source_filename: juma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 01:02:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: juma.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/juma/security/juma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Marketing
- Automation
- SaaS
- Advertising
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: focused.space
  spf: true
hosts:
- cert_expires: Sep 27 15:06:15 2026 GMT
  host: focused.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Focused Space Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Focused Space, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Focused Space, Inc.
provider_slug: focused-space-inc
slug: focused-space-inc-domain-security
source_filename: focused-space-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: focused.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:06:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: focused.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/focused-space-inc/refs/heads/main/security/focused-space-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Focus
- Body Doubling
- ADHD
- Remote Work
- Mental Health
- Consumer App
---

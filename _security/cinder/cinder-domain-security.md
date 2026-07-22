---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cinder.ai
  spf: true
hosts:
- cert_expires: Oct 10 12:55:25 2026 GMT
  host: cinder.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cinder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cinder
provider_slug: cinder
slug: cinder-domain-security
source_filename: cinder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cinder.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 12:55:25 2026 GMT\n  hsts: null\ndomains:\n- domain: cinder.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cinder/refs/heads/main/security/cinder-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Security
- Trust and Safety
- Content Moderation
- Policy Enforcement
- Moderation
- Artificial Intelligence
---

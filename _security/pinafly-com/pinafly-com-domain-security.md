---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pinafly.com
  spf: true
hosts:
- cert_expires: Dec  4 04:01:35 2026 GMT
  host: pinafly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pinafly Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pinafly-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: pinafly-com
provider_slug: pinafly-com
slug: pinafly-com-domain-security
source_filename: pinafly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pinafly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 04:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pinafly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pinafly-com/security/pinafly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Review
- AI
- Collaboration
- Feedback
- WebApp
---

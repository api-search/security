---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: praxislabs.co
  spf: true
hosts:
- cert_expires: Sep 14 18:04:36 2026 GMT
  host: praxislabs.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Praxislabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Praxis Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Praxis Labs
provider_slug: praxislabs
slug: praxislabs-domain-security
source_filename: praxislabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: praxislabs.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:04:36 2026 GMT\n  hsts: false\ndomains:\n- domain: praxislabs.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/praxislabs/refs/heads/main/security/praxislabs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Learning
- Leadership Development
- Corporate Training
- HR Tech
- AI Coaching
- Simulation
- SaaS
---

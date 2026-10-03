---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brainster.co
  spf: true
hosts:
- cert_expires: Dec 16 06:59:25 2026 GMT
  host: ai.brainster.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brainster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brainster
provider_slug: brainster
slug: brainster-domain-security
source_filename: brainster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai.brainster.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 06:59:25 2026 GMT\n  hsts: false\ndomains:\n- domain: brainster.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainster/refs/heads/main/security/brainster-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EdTech
- AI
- OnlineEducation
- Macedonia
- Training
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brainco.tech
  spf: true
hosts:
- cert_expires: Sep 25 23:22:30 2026 GMT
  host: www.brainco.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brainco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrainCo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BrainCo
provider_slug: brainco
slug: brainco-domain-security
source_filename: brainco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brainco.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:22:30 2026 GMT\n  hsts: false\ndomains:\n- domain: brainco.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainco/refs/heads/main/security/brainco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Neurotechnology
- Brain-Computer Interface
- EEG
- Wearables
- Robotics
- SDK
- Education
---

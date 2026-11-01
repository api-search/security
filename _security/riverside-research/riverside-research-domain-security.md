---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: riversideresearch.org
  spf: true
hosts:
- cert_expires: Jan 10 12:38:41 2027 GMT
  host: www.riversideresearch.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Riverside Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riverside Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Riverside Research
provider_slug: riverside-research
slug: riverside-research-domain-security
source_filename: riverside-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.riversideresearch.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 12:38:41 2027 GMT\n  hsts: false\ndomains:\n- domain: riversideresearch.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/riverside-research/security/riverside-research-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Nonprofit
- Research
- AI
- Plasma Physics
- Radar Systems
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cognicoree.tech
  spf: true
hosts:
- cert_expires: Jan 10 19:15:45 2027 GMT
  host: cognicoree.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CogniCore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CogniCore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CogniCore
provider_slug: cognicoree-tech
slug: cognicoree-tech-domain-security
source_filename: cognicoree-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognicoree.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 19:15:45 2027 GMT\n  hsts: false\ndomains:\n- domain: cognicoree.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cognicoree-tech/security/cognicoree-tech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Coding Agents
- Shared-Memory
- local-first storage
- cross‑agent sync
---

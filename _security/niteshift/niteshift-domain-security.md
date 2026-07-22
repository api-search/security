---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: niteshift.dev
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: niteshift.dev
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Niteshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Niteshift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Niteshift
provider_slug: niteshift
slug: niteshift-domain-security
source_filename: niteshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: niteshift.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: niteshift.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niteshift/refs/heads/main/security/niteshift-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Infrastructure
- Coding Agents
- AI Agents
- Developer Tools
- Cloud Development Environments
- DevOps
- Automation
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spacemaker.ai
  spf: true
hosts:
- cert_expires: Sep 22 12:59:33 2026 GMT
  host: spacemaker.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spacemaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spacemaker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spacemaker
provider_slug: spacemaker
slug: spacemaker-domain-security
source_filename: spacemaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spacemaker.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:59:33 2026 GMT\n  hsts: null\ndomains:\n- domain: spacemaker.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacemaker/refs/heads/main/security/spacemaker-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Real Estate
- Proptech
- Architecture
- Urban Planning
- Artificial Intelligence
- Generative Design
- Autodesk
---

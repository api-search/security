---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: systra.tools
  spf: true
hosts:
- cert_expires: Jan 18 20:27:49 2027 GMT
  host: systra.tools
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Systra Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Systra Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Systra Tools
provider_slug: systra-tools
slug: systra-tools-domain-security
source_filename: systra-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: systra.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 20:27:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: systra.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/systra-tools/security/systra-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- UI Components
- React
- Tailwind CSS
- AI Workflow
---

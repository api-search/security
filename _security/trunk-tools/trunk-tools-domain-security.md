---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trunktools.com
  spf: true
hosts:
- cert_expires: Sep 25 04:20:17 2026 GMT
  host: trunktools.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trunk Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trunk Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trunk Tools
provider_slug: trunk-tools
slug: trunk-tools-domain-security
source_filename: trunk-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trunktools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:20:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: trunktools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trunk-tools/refs/heads/main/security/trunk-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Construction Technology
- Artificial Intelligence
- Machine Learning
- Document Intelligence
- Workflow Automation
- SaaS
---

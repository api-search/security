---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 3dfortify.com
  spf: true
hosts:
- host: www.3dfortify.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3Dfortify Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortify, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fortify
provider_slug: 3dfortify-com
slug: 3dfortify-com-domain-security
source_filename: 3dfortify-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3dfortify.com\n  https: false\ndomains:\n- domain: 3dfortify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/3dfortify-com/security/3dfortify-com-domain-security.yml
summary_line: DMARC
tags:
- Security
- Application Security
- DevOps
- Vulnerability Management
- Cloud
---

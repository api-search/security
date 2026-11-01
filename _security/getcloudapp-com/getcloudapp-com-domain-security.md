---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getcloudapp.com
  spf: true
hosts:
- host: getcloudapp.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getcloudapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zight, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zight
provider_slug: getcloudapp-com
slug: getcloudapp-com-domain-security
source_filename: getcloudapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcloudapp.com\n  https: false\ndomains:\n- domain: getcloudapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getcloudapp-com/security/getcloudapp-com-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cloud
- Asset Management
- File Sharing
- Collaboration
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unified-grocers.com
  spf: false
hosts:
- host: www.unified-grocers.com
  https: false
kind: domain-security
layout: security
method: probed
name: Unified Grocers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unified Grocers, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Unified Grocers
provider_slug: unified-grocers
slug: unified-grocers-domain-security
source_filename: unified-grocers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unified-grocers.com\n  https: false\ndomains:\n- domain: unified-grocers.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unified-grocers/refs/heads/main/security/unified-grocers-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Grocery
- Wholesale
- Cooperative
- Retail
---

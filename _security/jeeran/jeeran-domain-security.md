---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: jeeran.com
  spf: false
hosts:
- host: jeeran.com
  https: false
kind: domain-security
layout: security
method: probed
name: Jeeran Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jeeran, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Jeeran
provider_slug: jeeran
slug: jeeran-domain-security
source_filename: jeeran-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jeeran.com\n  https: false\ndomains:\n- domain: jeeran.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jeeran/refs/heads/main/security/jeeran-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---

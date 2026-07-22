---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: helloenglish.com
  spf: false
hosts:
- host: helloenglish.com
  https: false
kind: domain-security
layout: security
method: probed
name: Intap Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intap Labs, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Intap Labs
provider_slug: intap-labs
slug: intap-labs-domain-security
source_filename: intap-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helloenglish.com\n  https: false\ndomains:\n- domain: helloenglish.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intap-labs/refs/heads/main/security/intap-labs-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---

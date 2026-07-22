---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: wegowhere.com
  spf: true
hosts:
- host: wegowhere.com
  https: false
kind: domain-security
layout: security
method: probed
name: Wegowhere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeGoWhere, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: WeGoWhere
provider_slug: wegowhere
slug: wegowhere-domain-security
source_filename: wegowhere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wegowhere.com\n  https: false\ndomains:\n- domain: wegowhere.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wegowhere/refs/heads/main/security/wegowhere-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Social
- Mobile App
- Social Networking
- Activity Planning
- Events
- Consumer
- Thailand
---

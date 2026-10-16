---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gosubscription.com
  spf: true
hosts:
- host: gosubscription.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Go Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Go, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Go
provider_slug: go
slug: go-domain-security
source_filename: go-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gosubscription.com\n  https: false\ndomains:\n- domain: gosubscription.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go/refs/heads/main/security/go-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---

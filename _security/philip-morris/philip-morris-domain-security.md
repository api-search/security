---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: philip-morris.com
  spf: true
hosts:
- host: www.philip-morris.com
  https: false
kind: domain-security
layout: security
method: probed
name: Philip Morris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for philip-morris, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: philip-morris
provider_slug: philip-morris
slug: philip-morris-domain-security
source_filename: philip-morris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.philip-morris.com\n  https: false\ndomains:\n- domain: philip-morris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philip-morris/refs/heads/main/security/philip-morris-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Fortune 500
---

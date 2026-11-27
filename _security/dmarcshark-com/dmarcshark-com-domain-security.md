---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dmarcshark.com
  spf: true
hosts:
- host: dmarcshark.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: dmarcshark-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dmarcshark-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: dmarcshark-com
provider_slug: dmarcshark-com
slug: dmarcshark-com-domain-security
source_filename: dmarcshark-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dmarcshark.com\n  https: false\ndomains:\n- domain: dmarcshark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dmarcshark-com/security/dmarcshark-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biosunpharma.com
  spf: true
hosts:
- host: biosunpharma.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biosunpharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biosunpharma, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Biosunpharma
provider_slug: biosunpharma
slug: biosunpharma-domain-security
source_filename: biosunpharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biosunpharma.com\n  https: false\ndomains:\n- domain: biosunpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biosunpharma/refs/heads/main/security/biosunpharma-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---

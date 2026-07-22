---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: encorealert.com
  spf: true
hosts:
- host: encorealert.com
  https: false
kind: domain-security
layout: security
method: probed
name: Encore Hq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Encore HQ, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Encore HQ
provider_slug: encore-hq
slug: encore-hq-domain-security
source_filename: encore-hq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: encorealert.com\n  https: false\ndomains:\n- domain: encorealert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encore-hq/refs/heads/main/security/encore-hq-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aylien.com
  spf: true
hosts:
- host: docs.aylien.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aylien Text Analysis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aylien Text Analysis, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aylien Text Analysis
provider_slug: aylien-text-analysis
slug: aylien-text-analysis-domain-security
source_filename: aylien-text-analysis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aylien.com\n  https: false\ndomains:\n- domain: aylien.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aylien-text-analysis/refs/heads/main/security/aylien-text-analysis-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Text Analysis
- Public APIs
---

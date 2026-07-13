---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: govdata.de
  spf: true
hosts:
- host: www.govdata.de
  https: false
kind: domain-security
layout: security
method: probed
name: Open Government Germany Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Germany, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Open Government, Germany
provider_slug: open-government-germany
slug: open-government-germany-domain-security
source_filename: open-government-germany-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.govdata.de\n  https: false\ndomains:\n- domain: govdata.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-germany/refs/heads/main/security/open-government-germany-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Government
- Public APIs
---

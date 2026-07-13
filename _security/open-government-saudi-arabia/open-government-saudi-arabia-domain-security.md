---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: data.gov.sa
  spf: false
hosts:
- host: data.gov.sa
  https: false
kind: domain-security
layout: security
method: probed
name: Open Government Saudi Arabia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Saudi Arabia, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Open Government, Saudi Arabia
provider_slug: open-government-saudi-arabia
slug: open-government-saudi-arabia-domain-security
source_filename: open-government-saudi-arabia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.sa\n  https: false\ndomains:\n- domain: data.gov.sa\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-saudi-arabia/refs/heads/main/security/open-government-saudi-arabia-domain-security.yml
summary_line: DNSSEC
tags:
- Government
- Public APIs
---

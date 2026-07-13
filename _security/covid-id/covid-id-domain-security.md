---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: go.id
  spf: false
hosts:
- host: data.covid19.go.id
  https: false
kind: domain-security
layout: security
method: probed
name: Covid Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COVID-ID, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: COVID-ID
provider_slug: covid-id
slug: covid-id-domain-security
source_filename: covid-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.covid19.go.id\n  https: false\ndomains:\n- domain: go.id\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covid-id/refs/heads/main/security/covid-id-domain-security.yml
summary_line: DNSSEC
tags:
- Health
- Public APIs
---

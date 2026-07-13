---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clickmeter.com
  spf: true
hosts:
- host: support.clickmeter.com
  https: false
kind: domain-security
layout: security
method: probed
name: Clickmeter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClickMeter, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ClickMeter
provider_slug: clickmeter
slug: clickmeter-domain-security
source_filename: clickmeter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: support.clickmeter.com\n  https: false\ndomains:\n- domain: clickmeter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickmeter/refs/heads/main/security/clickmeter-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- URL Shorteners
- Public APIs
---

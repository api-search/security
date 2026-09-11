---
api_specs:
- filename: openapi.json
  format: json
  label: Unicorn Screener API
  slug: unicorn-screener-api
  spec_type: OpenAPI
  url: https://unicornscreener.vc/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unicornscreener.vc
  spf: true
hosts:
- cert_expires: Nov 19 19:59:10 2026 GMT
  host: unicornscreener.vc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unicorn Screener Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unicorn Screener, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unicorn Screener
provider_slug: unicorn-screener
slug: unicorn-screener-domain-security
source_filename: unicorn-screener-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unicornscreener.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 19:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: unicornscreener.vc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicorn-screener/refs/heads/main/security/unicorn-screener-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Venture Capital
- Startups
- Company Research
- Screening
- Investing
- AI Agents
---

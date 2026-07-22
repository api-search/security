---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seekingalpha.com
  spf: true
hosts:
- cert_expires: Jan 10 01:00:30 2027 GMT
  host: seekingalpha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seekingalpha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SeekingAlpha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SeekingAlpha
provider_slug: seekingalpha
slug: seekingalpha-domain-security
source_filename: seekingalpha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seekingalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:00:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seekingalpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seekingalpha/refs/heads/main/security/seekingalpha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social
- Finance
- Investing
- Stock Market
- Financial Research
- Media
---

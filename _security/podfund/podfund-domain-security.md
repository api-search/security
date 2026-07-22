---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pod.fund
  spf: true
hosts:
- cert_expires: Oct 16 02:39:51 2026 GMT
  host: pod.fund
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podfund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podfund, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Podfund
provider_slug: podfund
slug: podfund-domain-security
source_filename: podfund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pod.fund\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 02:39:51 2026 GMT\n  hsts: false\ndomains:\n- domain: pod.fund\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podfund/refs/heads/main/security/podfund-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Venture Capital
- Podcasting
- Media
- Funding
- Investment
- Audio
- Creators
---

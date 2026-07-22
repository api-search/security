---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: skvcap.com
  spf: true
hosts:
- cert_expires: Oct  2 06:30:11 2026 GMT
  host: skvcap.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sk Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SK Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SK Ventures
provider_slug: sk-ventures
slug: sk-ventures-domain-security
source_filename: sk-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skvcap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:30:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: skvcap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sk-ventures/refs/heads/main/security/sk-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Venture Capital
- Investors
- Seed Stage
- Startups
- Technology
- Infrastructure
- Identity
---

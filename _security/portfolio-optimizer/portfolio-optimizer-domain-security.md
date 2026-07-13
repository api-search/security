---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: portfoliooptimizer.io
  spf: true
hosts:
- cert_expires: Aug 20 05:20:41 2026 GMT
  host: portfoliooptimizer.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Portfolio Optimizer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portfolio Optimizer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Portfolio Optimizer
provider_slug: portfolio-optimizer
slug: portfolio-optimizer-domain-security
source_filename: portfolio-optimizer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portfoliooptimizer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 05:20:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: portfoliooptimizer.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portfolio-optimizer/refs/heads/main/security/portfolio-optimizer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Finance
- Public APIs
---

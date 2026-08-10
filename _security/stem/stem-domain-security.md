---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stemai.vc
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: stemai.vc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stem AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Stem AI
provider_slug: stem
slug: stem-domain-security
source_filename: stem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stemai.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: stemai.vc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stem/refs/heads/main/security/stem-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Venture Capital
- Accelerator
- Artificial Intelligence
- Large Language Models
- Startups
- France
- Investment
---

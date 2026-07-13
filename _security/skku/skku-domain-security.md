---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skku.edu
  spf: true
hosts:
- cert_expires: Jul 25 23:59:59 2026 GMT
  host: www.skku.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sungkyunkwan University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sungkyunkwan University
provider_slug: skku
slug: skku-domain-security
source_filename: skku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skku.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: skku.edu\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skku/refs/heads/main/security/skku-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- South Korea
- Seoul
---

---
description: ''
domains:
- caa:
  - dqcq79cfzkeej.cloudfront.net.
  dmarc: false
  dnssec: true
  domain: gmr.xyz
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: gmr.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gmr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GMR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: GMR
provider_slug: gmr
slug: gmr-domain-security
source_filename: gmr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gmr.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gmr.xyz\n  dnssec: true\n  caa:\n  - dqcq79cfzkeej.cloudfront.net.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gmr/refs/heads/main/security/gmr-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Crypto Web3
- Mining
- Research
- Blockchain
---

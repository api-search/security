---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bittrex.com
  spf: true
hosts:
- cert_expires: Nov 30 06:47:32 2026 GMT
  host: bittrex.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bittrexllc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bittrexllc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bittrexllc
provider_slug: bittrexllc
slug: bittrexllc-domain-security
source_filename: bittrexllc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bittrex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 30 06:47:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: bittrex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bittrexllc/refs/heads/main/security/bittrexllc-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
---

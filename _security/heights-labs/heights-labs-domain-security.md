---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: heightslabs.com
  spf: true
hosts:
- cert_expires: Aug 13 11:06:38 2026 GMT
  host: www.heightslabs.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heights Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heights Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Heights Labs
provider_slug: heights-labs
slug: heights-labs-domain-security
source_filename: heights-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heightslabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 11:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: heightslabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heights-labs/refs/heads/main/security/heights-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto
- Blockchain
- Web3
- Fintech
---

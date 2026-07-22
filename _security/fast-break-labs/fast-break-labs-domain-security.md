---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: fastbreaklabs.com
  spf: true
hosts:
- host: www.fastbreaklabs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fast Break Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fast Break Labs, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Fast Break Labs
provider_slug: fast-break-labs
slug: fast-break-labs-domain-security
source_filename: fast-break-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fastbreaklabs.com\n  https: false\ndomains:\n- domain: fastbreaklabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fast-break-labs/refs/heads/main/security/fast-break-labs-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Crypto
- Blockchain
- Web3
- Venture Backed
---

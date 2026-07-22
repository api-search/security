---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cega.fi
  spf: true
hosts:
- host: www.cega.fi
  https: false
kind: domain-security
layout: security
method: probed
name: Cega Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cega, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cega
provider_slug: cega
slug: cega-domain-security
source_filename: cega-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cega.fi\n  https: false\ndomains:\n- domain: cega.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cega/refs/heads/main/security/cega-domain-security.yml
summary_line: DMARC
tags:
- Company
- Crypto
- DeFi
- Derivatives
- Options
- Structured Products
- Blockchain
- Solana
- Ethereum
- SDK
---

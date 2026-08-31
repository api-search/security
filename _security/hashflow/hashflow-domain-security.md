---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hashflow.com
  spf: true
hosts:
- cert_expires: Sep 19 07:09:44 2026 GMT
  host: www.hashflow.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hashflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hashflow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hashflow
provider_slug: hashflow
slug: hashflow-domain-security
source_filename: hashflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hashflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:09:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hashflow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashflow/refs/heads/main/security/hashflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defi
- DEX
- RFQ
- Trading
- Crypto
- Market Making
- Cross-Chain
- Blockchain
- Web3
---

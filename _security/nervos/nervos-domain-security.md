---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nervos.org
  spf: true
hosts:
- cert_expires: Sep 15 06:09:40 2026 GMT
  host: nervos.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nervos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nervos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nervos
provider_slug: nervos
slug: nervos-domain-security
source_filename: nervos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nervos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:09:40 2026 GMT\n  hsts: null\ndomains:\n- domain: nervos.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nervos/refs/heads/main/security/nervos-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- Layer 1
- JSON-RPC
- Smart Contracts
- Web3 Infrastructure
- Developer Tools
---

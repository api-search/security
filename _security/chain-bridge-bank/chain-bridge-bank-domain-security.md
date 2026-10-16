---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chainbridgebank.com
  spf: true
hosts:
- cert_expires: Jan  3 19:06:18 2027 GMT
  host: www.chainbridgebank.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chain Bridge Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chain Bridge Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chain Bridge Bank
provider_slug: chain-bridge-bank
slug: chain-bridge-bank-domain-security
source_filename: chain-bridge-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chainbridgebank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 19:06:18 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: chainbridgebank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chain-bridge-bank/refs/heads/main/security/chain-bridge-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Financial Services
- Commercial Banking
- Trust Services
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 5ire.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: 5ire.network
  spf: false
hosts:
- cert_expires: Sep 25 06:47:56 2026 GMT
  host: 5ire.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 06:47:56 2026 GMT
  host: docs.5ire.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 09:26:47 2026 GMT
  host: rpc.5ire.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 5Ire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 5ire, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 5ire
provider_slug: 5ire
slug: 5ire-domain-security
source_filename: 5ire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 5ire.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:47:56 2026 GMT\n  hsts: null\n- host: docs.5ire.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:47:56 2026 GMT\n  hsts: null\n- host: rpc.5ire.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:26:47 2026 GMT\n  hsts: null\ndomains:\n- domain: 5ire.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: 5ire.network\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/5ire/refs/heads/main/security/5ire-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- blockchain
- layer-1
- smart-contracts
- evm
- web3
- substrate
- json-rpc
- sustainability
- esg
- proof-of-stake
- cryptocurrency
- developer-tools
---

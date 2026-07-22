---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zama.org
  spf: true
hosts:
- cert_expires: Sep 23 03:33:23 2026 GMT
  host: www.zama.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zama
provider_slug: zama
slug: zama-domain-security
source_filename: zama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zama.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:33:23 2026 GMT\n  hsts: false\ndomains:\n- domain: zama.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zama/refs/heads/main/security/zama-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- Cryptography
- Fully Homomorphic Encryption
- FHE
- Privacy
- Blockchain
- Smart Contracts
- Machine Learning
- Open Source
- SDKs
---

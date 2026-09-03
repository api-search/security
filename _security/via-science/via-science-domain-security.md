---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: solvewithvia.com
  spf: true
hosts:
- cert_expires: Oct 22 10:38:57 2026 GMT
  host: www.solvewithvia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: documentation.ztf.solvewithvia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 26 04:15:25 2026 GMT
  host: auth.solvewithvia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Via Science Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Via Science, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Via Science
provider_slug: via-science
slug: via-science-domain-security
source_filename: via-science-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solvewithvia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 10:38:57 2026 GMT\n  hsts: false\n- host: documentation.ztf.solvewithvia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.solvewithvia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 04:15:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: solvewithvia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/via-science/refs/heads/main/security/via-science-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Identity
- Authentication
- Zero Trust
- Decentralized Identity
- Verifiable Credentials
- Post-Quantum Cryptography
- Encryption
- File Transfer
- Defense
- Artificial Intelligence
- Blockchain
- OpenID Connect
---

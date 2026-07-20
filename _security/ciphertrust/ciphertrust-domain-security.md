---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thalesgroup.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: cpl.thalesgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 17:17:26 2026 GMT
  host: docs-cybersec.thalesgroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ciphertrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CipherTrust, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CipherTrust
provider_slug: ciphertrust
slug: ciphertrust-domain-security
source_filename: ciphertrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cpl.thalesgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs-cybersec.thalesgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:17:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thalesgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciphertrust/refs/heads/main/security/ciphertrust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Encryption
- Key Management
- Secrets Management
- Data Protection
- Cryptography
- Tokenization
- Compliance
- KMIP
---

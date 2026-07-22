---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:certificate-abuse@kraken.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: staked.us
  spf: true
hosts:
- cert_expires: Sep 19 21:21:07 2026 GMT
  host: staked.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Staked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Staked, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Staked
provider_slug: staked
slug: staked-domain-security
source_filename: staked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: staked.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: staked.us\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:certificate-abuse@kraken.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/staked/refs/heads/main/security/staked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Staking
- Blockchain
- Ethereum
- Proof of Stake
- Validator
- Institutional
---

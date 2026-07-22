---
description: ''
domains:
- caa:
  - 128 issue "pki.goog"
  - 128 iodef "mailto:security@forte.io"
  - 128 issue "amazon.com"
  - 128 issue "cloudflare.com"
  - 128 issue "godaddy.com"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: forte.io
  spf: true
hosts:
- cert_expires: Oct 15 15:26:39 2026 GMT
  host: www.forte.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forte Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forte Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Forte Labs
provider_slug: forte-labs
slug: forte-labs-domain-security
source_filename: forte-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.forte.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:26:39 2026 GMT\n  hsts: false\ndomains:\n- domain: forte.io\n  dnssec: false\n  caa:\n  - 128 issue \"pki.goog\"\n  - 128 iodef \"mailto:security@forte.io\"\n  - 128 issue \"amazon.com\"\n  - 128 issue \"cloudflare.com\"\n  - 128 issue \"godaddy.com\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forte-labs/refs/heads/main/security/forte-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Blockchain
- Web3
- Compliance
- Smart Contracts
- Gaming
- Developer Tools
- SDK
- EVM
- On-Chain Governance
---

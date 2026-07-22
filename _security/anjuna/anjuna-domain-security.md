---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:it@anjna.io"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: anjuna.io
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.anjuna.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anjuna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anjuna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Anjuna
provider_slug: anjuna
slug: anjuna-domain-security
source_filename: anjuna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anjuna.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anjuna.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:it@anjna.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anjuna/refs/heads/main/security/anjuna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Confidential Computing
- Security
- Cloud
- Encryption
- Trusted Execution Environment
- Attestation
- AI Governance
---

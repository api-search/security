---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keyfactor.com
  spf: true
hosts:
- cert_expires: Oct 16 18:59:19 2026 GMT
  host: www.keyfactor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keyfactor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keyfactor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Keyfactor
provider_slug: keyfactor
slug: keyfactor-domain-security
source_filename: keyfactor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keyfactor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 18:59:19 2026 GMT\n  hsts: null\ndomains:\n- domain: keyfactor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyfactor/refs/heads/main/security/keyfactor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- PKI
- Machine Identity
- Certificate Lifecycle
- Code Signing
- Cryptography
- Digital Trust
- Security
---

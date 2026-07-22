---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: key.me
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: key.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keyme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeyMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KeyMe
provider_slug: keyme
slug: keyme-domain-security
source_filename: keyme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: key.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: key.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyme/refs/heads/main/security/keyme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Locksmith
- Key Duplication
- Kiosks
- Security
- Access Control
- Retail
- Consumer Services
---

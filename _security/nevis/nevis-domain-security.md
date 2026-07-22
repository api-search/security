---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nevis.net
  spf: true
hosts:
- cert_expires: Sep  9 00:08:25 2026 GMT
  host: www.nevis.net
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 10:34:02 2026 GMT
  host: docs.nevis.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nevis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nevis, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nevis
provider_slug: nevis
slug: nevis-domain-security
source_filename: nevis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nevis.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:08:25 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: docs.nevis.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:34:02 2026 GMT\n  hsts: false\ndomains:\n- domain: nevis.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nevis/refs/heads/main/security/nevis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Authentication
- Identity
- Passwordless
- FIDO2
- Passkeys
- CIAM
- Transaction Signing
- Security
---

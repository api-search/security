---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: proof.com
  spf: true
hosts:
- cert_expires: Sep 30 04:18:45 2026 GMT
  host: www.proof.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 22 09:25:07 2026 GMT
  host: dev.proof.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.proof.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Notarize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notarize, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Notarize
provider_slug: notarize
slug: notarize-domain-security
source_filename: notarize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proof.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 04:18:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.proof.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 09:25:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.proof.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: proof.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/security/notarize-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Proptech
- Notarization
- Remote Online Notarization
- Identity Verification
- eSignature
- Digital Credentials
- Real Estate
- Mortgage
- Legal Tech
---

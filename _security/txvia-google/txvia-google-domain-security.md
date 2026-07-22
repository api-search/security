---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: txvia.com
  spf: true
hosts:
- cert_expires: Sep 21 08:38:00 2026 GMT
  host: www.txvia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Txvia Google Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TxVia (Google), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TxVia (Google)
provider_slug: txvia-google
slug: txvia-google-domain-security
source_filename: txvia-google-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.txvia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:38:00 2026 GMT\n  hsts: false\ndomains:\n- domain: txvia.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/txvia-google/refs/heads/main/security/txvia-google-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- Prepaid Cards
- Payment Processing
- Issuer Processing
- Acquired
---

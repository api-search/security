---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cosmolex.com
  spf: true
hosts:
- cert_expires: Aug 20 10:13:23 2026 GMT
  host: www.cosmolex.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: law.cosmolex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cosmolex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CosmoLex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CosmoLex
provider_slug: cosmolex
slug: cosmolex-domain-security
source_filename: cosmolex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cosmolex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: law.cosmolex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cosmolex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmolex/refs/heads/main/security/cosmolex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Law Practice Management
- Matter Management
- Billing
- Trust Accounting
- Time Tracking
- Legal Compliance
- Legal Software
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flywire.com
  spf: true
hosts:
- cert_expires: Sep 14 02:47:36 2026 GMT
  host: www.flywire.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 02:47:36 2026 GMT
  host: developers.flywire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 02:47:36 2026 GMT
  host: api-platform.flywire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flywire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flywire, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flywire
provider_slug: flywire
slug: flywire-domain-security
source_filename: flywire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flywire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:47:36 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: developers.flywire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:47:36 2026 GMT\n  hsts: false\n- host: api-platform.flywire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:47:36 2026 GMT\n  hsts: null\ndomains:\n- domain: flywire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flywire/refs/heads/main/security/flywire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Cross-Border Payments
- FinTech
- Education Payments
- Healthcare Payments
- Travel Payments
- B2B Payments
- Checkout
- Webhooks
---

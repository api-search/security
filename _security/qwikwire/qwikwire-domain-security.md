---
description: ''
domains:
- caa:
  - 0 iodef "mailto:developers@qwikwire.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aqwire.io
  spf: true
hosts:
- cert_expires: Sep 29 02:11:41 2026 GMT
  host: aqwire.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:45:19 2026 GMT
  host: developers.aqwire.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 15:48:22 2026 GMT
  host: api.aqwire.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qwikwire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qwikwire, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Qwikwire
provider_slug: qwikwire
slug: qwikwire-domain-security
source_filename: qwikwire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aqwire.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:11:41 2026 GMT\n  hsts: false\n- host: developers.aqwire.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:45:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aqwire.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:48:22 2026 GMT\n  hsts: null\ndomains:\n- domain: aqwire.io\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:developers@qwikwire.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwikwire/refs/heads/main/security/qwikwire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Cross-Border Payments
- Real Estate
- FinTech
- Philippines
- Multi-Currency
- Remittance
---

---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:abuse@quickpay.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quickpay.net
  spf: true
hosts:
- cert_expires: Dec 27 10:55:16 2026 GMT
  host: quickpay.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quickpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quickpay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quickpay
provider_slug: quickpay
slug: quickpay-domain-security
source_filename: quickpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickpay.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 10:55:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quickpay.net\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:abuse@quickpay.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/quickpay/security/quickpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- API
- FinTech
- European
- E‑commerce
---

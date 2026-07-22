---
description: ''
domains:
- caa:
  - 0 iodef "mailto:hello@kema.co"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kema.co
  spf: true
hosts:
- cert_expires: Oct 14 17:47:07 2026 GMT
  host: kema.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kema Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kema, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kema
provider_slug: kema
slug: kema-domain-security
source_filename: kema-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kema.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:47:07 2026 GMT\n  hsts: null\ndomains:\n- domain: kema.co\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hello@kema.co\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kema/refs/heads/main/security/kema-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- Invoice Financing
- Accounts Receivable
- B2B Payments
- Cash Flow
- Working Capital
- Payment Links
- MENA
- SME
---

---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:contact@paywholesail.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: paywholesail.com
  spf: true
hosts:
- cert_expires: Sep  1 20:48:12 2026 GMT
  host: www.paywholesail.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wholesail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wholesail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Wholesail
provider_slug: wholesail
slug: wholesail-domain-security
source_filename: wholesail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paywholesail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paywholesail.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:contact@paywholesail.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wholesail/refs/heads/main/security/wholesail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Accounts Receivable
- B2B
- ACH
- Wholesale
- Collections
---

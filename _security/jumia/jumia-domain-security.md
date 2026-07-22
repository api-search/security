---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jumia.com
  spf: true
hosts:
- cert_expires: Aug 16 02:08:38 2026 GMT
  host: group.jumia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jumia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jumia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jumia
provider_slug: jumia
slug: jumia-domain-security
source_filename: jumia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: group.jumia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 02:08:38 2026 GMT\n  hsts: false\ndomains:\n- domain: jumia.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jumia/refs/heads/main/security/jumia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Ecommerce
- Marketplace
- Africa
- Pan-African
- Retail
- Payments
- Logistics
- Vendor Management
- Sellers
- Merchant Services
- Mobile Commerce
- Emerging Markets
- Public Company
---

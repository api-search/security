---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chippercash.com
  spf: true
hosts:
- cert_expires: Aug 26 21:12:04 2026 GMT
  host: www.chippercash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chipper Cash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chipper Cash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chipper Cash
provider_slug: chipper-cash
slug: chipper-cash-domain-security
source_filename: chipper-cash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chippercash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chippercash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chipper-cash/refs/heads/main/security/chipper-cash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Africa
- Cross Border Payments
- Money Transfer
- Remittances
- Mobile Money
- Digital Wallet
- Virtual Cards
- Bill Pay
- Airtime
- Crypto
- Investing
- Fractional Shares
- Identity Verification
- Merchant Payments
- Payouts
- Network API
- Pay With Chipper
- tbDEX
- Unicorn
- Nigeria
- Ghana
- Uganda
- Tanzania
- South Africa
- Rwanda
- United Kingdom
- United States
---

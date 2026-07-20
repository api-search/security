---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: beamcheckout.com
  spf: true
hosts:
- cert_expires: Oct  2 02:07:02 2026 GMT
  host: www.beamcheckout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beam Checkout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beam Checkout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Beam Checkout
provider_slug: beam-checkout
slug: beam-checkout-domain-security
source_filename: beam-checkout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beamcheckout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:07:02 2026 GMT\n  hsts: false\ndomains:\n- domain: beamcheckout.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beam-checkout/refs/heads/main/security/beam-checkout-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Payments
- Checkout
- Card Payments
- Webhooks
- Thailand
- Fintech
---

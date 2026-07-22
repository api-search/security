---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: paynimo.com
  spf: true
hosts:
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: www.paynimo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Techprocess Payment Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TechProcess Payment Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TechProcess Payment Services
provider_slug: techprocess-payment-services
slug: techprocess-payment-services-domain-security
source_filename: techprocess-payment-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paynimo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: paynimo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/techprocess-payment-services/refs/heads/main/security/techprocess-payment-services-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Payment Gateway
- Financial Services
- India
- Checkout
- E-commerce
- NACH
---

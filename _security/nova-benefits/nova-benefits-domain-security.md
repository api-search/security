---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: novabenefits.com
  spf: true
hosts:
- cert_expires: Sep  5 06:38:21 2026 GMT
  host: novabenefits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nova Benefits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nova Benefits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nova Benefits
provider_slug: nova-benefits
slug: nova-benefits-domain-security
source_filename: nova-benefits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novabenefits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 06:38:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: novabenefits.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova-benefits/refs/heads/main/security/nova-benefits-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Insurance
- Employee Benefits
- Health Insurance
- Wellness
- InsurTech
- India
---

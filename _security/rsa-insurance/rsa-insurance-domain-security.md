---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rsainsurance.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intactinsurance.co.uk
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.rsainsurance.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: www.intactinsurance.co.uk
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.rsaconnect.rsagroup.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rsa Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RSA Insurance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RSA Insurance
provider_slug: rsa-insurance
slug: rsa-insurance-domain-security
source_filename: rsa-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rsainsurance.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.intactinsurance.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.rsaconnect.rsagroup.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rsainsurance.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: intactinsurance.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsa-insurance/refs/heads/main/security/rsa-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Commercial Lines
- Carrier
- Brokers
- Claims
- Underwriting
- Partner Gated
---

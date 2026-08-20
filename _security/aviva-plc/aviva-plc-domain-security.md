---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aviva.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aviva.co.uk
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.aviva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.aviva.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: connect.avivab2b.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aviva Plc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aviva plc, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aviva plc
provider_slug: aviva-plc
slug: aviva-plc-domain-security
source_filename: aviva-plc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aviva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.aviva.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.avivab2b.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aviva.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: aviva.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviva-plc/refs/heads/main/security/aviva-plc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Life Insurance
- Health Insurance
- Claims
- Underwriting
- Brokers
- Workplace Pensions
- Carrier
---

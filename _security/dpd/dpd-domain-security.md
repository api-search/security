---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dpd.com
  spf: true
hosts:
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: www.dpd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dpd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DPD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DPD
provider_slug: dpd
slug: dpd-domain-security
source_filename: dpd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dpd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dpd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dpd/refs/heads/main/security/dpd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Logistics
- Parcel Delivery
- International Shipping
- E-Commerce
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chronopost.fr
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.chronopost.fr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chronopost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chronopost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chronopost
provider_slug: chronopost
slug: chronopost-domain-security
source_filename: chronopost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chronopost.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: chronopost.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chronopost/refs/heads/main/security/chronopost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Shipping
- Logistics
- Parcel Delivery
- Express Courier
- SOAP
- Tracking
- France
---

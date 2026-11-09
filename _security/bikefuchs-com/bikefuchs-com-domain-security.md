---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bikefuchs.com
  spf: false
hosts:
- cert_expires: Jan  1 10:13:14 2027 GMT
  host: bikefuchs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bikefuchs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bikefuchs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Bikefuchs
provider_slug: bikefuchs-com
slug: bikefuchs-com-domain-security
source_filename: bikefuchs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bikefuchs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 10:13:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bikefuchs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bikefuchs-com/security/bikefuchs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- E-Commerce
- Price Comparison
- Bicycles
- Shopping
---

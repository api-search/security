---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thredup.com
  spf: true
hosts:
- cert_expires: Sep 13 03:22:44 2026 GMT
  host: www.thredup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thredup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThredUp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ThredUp
provider_slug: thredup
slug: thredup-domain-security
source_filename: thredup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thredup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:22:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thredup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thredup/refs/heads/main/security/thredup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Resale
- Secondhand
- Fashion
- Consignment
- Sustainability
- Retail
---

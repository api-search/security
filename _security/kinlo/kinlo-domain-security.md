---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kinlo.com
  spf: true
hosts:
- cert_expires: Sep  5 05:56:01 2026 GMT
  host: kinlo.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kinlo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinlo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kinlo
provider_slug: kinlo
slug: kinlo-domain-security
source_filename: kinlo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kinlo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: kinlo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinlo/refs/heads/main/security/kinlo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Skincare
- Suncare
- Beauty
- SPF
- Ecommerce
- Direct-to-Consumer
---

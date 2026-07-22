---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tezbor.uz
  spf: true
hosts:
- cert_expires: Aug 28 02:27:42 2026 GMT
  host: tezbor.uz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tezbor Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tezbor, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tezbor, Inc.
provider_slug: tezbor-inc
slug: tezbor-inc-domain-security
source_filename: tezbor-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tezbor.uz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:27:42 2026 GMT\n  hsts: false\ndomains:\n- domain: tezbor.uz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tezbor-inc/refs/heads/main/security/tezbor-inc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Logistics
- Delivery
- Courier
- Shipping
- Last Mile
- E-commerce
- Uzbekistan
---

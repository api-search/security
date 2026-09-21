---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goairmart.com
  spf: true
hosts:
- cert_expires: Dec 10 03:42:58 2026 GMT
  host: www.goairmart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Airmart
provider_slug: airmart
slug: airmart-domain-security
source_filename: airmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goairmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 03:42:58 2026 GMT\n  hsts: false\ndomains:\n- domain: goairmart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airmart/refs/heads/main/security/airmart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Commerce
- Online Storefront
- Social Commerce
- Payments
- Delivery
- Small Business
- Food
- United States
- Company
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: justo.mx
  spf: true
hosts:
- cert_expires: Sep 12 17:00:53 2026 GMT
  host: justo.mx
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: J Sto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jüsto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jüsto
provider_slug: j-sto
slug: j-sto-domain-security
source_filename: j-sto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justo.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:00:53 2026 GMT\n  hsts: null\ndomains:\n- domain: justo.mx\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/j-sto/refs/heads/main/security/j-sto-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Grocery
- E-commerce
- Retail
- Food Delivery
- Consumer
- Mexico
- Latin America
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thelafz.com
  spf: false
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: lafz.com
  spf: false
hosts:
- cert_expires: Sep 29 22:45:25 2026 GMT
  host: thelafz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 12:12:32 2026 GMT
  host: lafz.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Lafz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Lafz, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: The Lafz
provider_slug: the-lafz
slug: the-lafz-domain-security
source_filename: the-lafz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thelafz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:45:25 2026 GMT\n  hsts: false\n- host: lafz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 12:12:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: thelafz.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: lafz.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-lafz/refs/heads/main/security/the-lafz-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Cosmetics
- Personal Care
- E-Commerce
- Halal
- Shopify
- Agent Commerce
---

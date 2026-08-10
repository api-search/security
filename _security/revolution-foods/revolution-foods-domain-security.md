---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: revolutionfoods.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: revfoods.com
  note: DMARC rua/ruf report to revolutionfoods.com addresses
  spf: true
hosts:
- cert_expires: Nov  1 11:56:58 2026 GMT
  host: www.revolutionfoods.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: centro.order.revfoods.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Centro customer ordering portal; root 302s to /Identity/Account/Login
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revolution Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revolution Foods, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Revolution Foods
provider_slug: revolution-foods
slug: revolution-foods-domain-security
source_filename: revolution-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revolutionfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 11:56:58 2026 GMT\n  hsts: false\n- host: centro.order.revfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: Centro customer ordering portal; root 302s to /Identity/Account/Login\ndomains:\n- domain: revolutionfoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: revfoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: DMARC rua/ruf report to revolutionfoods.com addresses\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolution-foods/refs/heads/main/security/revolution-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food
- Food Service
- Nutrition
- Meal Delivery
- Education
- K-12
- Schools
- Senior Services
- B Corporation
- Public Benefit Corporation
---

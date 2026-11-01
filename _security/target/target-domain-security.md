---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:certificate.management@target.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: target.com
  spf: true
hosts:
- cert_expires: Mar 11 12:56:33 2027 GMT
  host: www.target.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 15:20:11 2026 GMT
  host: tech.target.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 15:20:11 2026 GMT
  host: redsky.target.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Target Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Target, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Target
provider_slug: target
slug: target-domain-security
source_filename: target-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 12:56:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tech.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 15:20:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: redsky.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 15:20:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: target.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:certificate.management@target.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/target/security/target-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- E-Commerce
- Retail
- Product
- Inventory
- Stores
- Order
---

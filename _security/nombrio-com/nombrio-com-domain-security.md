---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: nombrio.com
  spf: true
hosts:
- cert_expires: Jan  5 07:20:24 2027 GMT
  host: nombrio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nombrio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nombrio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nombrio
provider_slug: nombrio-com
slug: nombrio-com-domain-security
source_filename: nombrio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nombrio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 07:20:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nombrio.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nombrio-com/security/nombrio-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Brands
- Naming
- Trademarks
- Domain
- Social
---

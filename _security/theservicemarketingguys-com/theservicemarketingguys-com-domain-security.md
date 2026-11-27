---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: theservicemarketingguys.com
  spf: true
hosts:
- cert_expires: Feb 12 18:11:18 2027 GMT
  host: theservicemarketingguys.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Service Marketing Guys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Service Marketing Guys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Service Marketing Guys
provider_slug: theservicemarketingguys-com
slug: theservicemarketingguys-com-domain-security
source_filename: theservicemarketingguys-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theservicemarketingguys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 18:11:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: theservicemarketingguys.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/theservicemarketingguys-com/security/theservicemarketingguys-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Home Services
- Service Business Software
---

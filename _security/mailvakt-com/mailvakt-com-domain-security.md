---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mailvakt.com
  spf: true
hosts:
- cert_expires: Jan 11 19:26:42 2027 GMT
  host: mailvakt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MailVakt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailVakt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MailVakt
provider_slug: mailvakt-com
slug: mailvakt-com-domain-security
source_filename: mailvakt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailvakt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 19:26:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailvakt.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mailvakt-com/security/mailvakt-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Deliverability
- Domain Check
- SPF
- DKIM
- DMARC
- Campaign Analytics
- Integration
---

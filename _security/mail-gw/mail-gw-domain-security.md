---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: mail.gw
  spf: true
hosts:
- cert_expires: Sep 15 18:55:40 2026 GMT
  host: docs.mail.gw
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mail Gw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mail.gw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: mail.gw
provider_slug: mail-gw
slug: mail-gw-domain-security
source_filename: mail-gw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.mail.gw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:55:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mail.gw\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mail-gw/refs/heads/main/security/mail-gw-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Email
- Public APIs
---

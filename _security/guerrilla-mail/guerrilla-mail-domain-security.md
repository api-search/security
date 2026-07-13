---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: guerrillamail.com
  spf: true
hosts:
- cert_expires: Aug 18 00:41:16 2026 GMT
  host: www.guerrillamail.com
  hsts: true
  hsts_max_age: 1
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Guerrilla Mail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guerrilla Mail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Guerrilla Mail
provider_slug: guerrilla-mail
slug: guerrilla-mail-domain-security
source_filename: guerrilla-mail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guerrillamail.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 00:41:16 2026 GMT\n  hsts: true\n  hsts_max_age: 1\ndomains:\n- domain: guerrillamail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guerrilla-mail/refs/heads/main/security/guerrilla-mail-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Email
- Public APIs
---

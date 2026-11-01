---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mail.ru
  spf: true
hosts:
- cert_expires: Dec 26 10:20:39 2026 GMT
  host: mail.ru
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mail Ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mail.ru Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mail.ru Cloud
provider_slug: mail-ru
slug: mail-ru-domain-security
source_filename: mail-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mail.ru\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 10:20:39 2026 GMT\n  hsts: false\ndomains:\n- domain: mail.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mail-ru/security/mail-ru-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Cloud
- Storage
- Collaboration
- Russian
- Email
---

---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yandex.com
  spf: true
hosts:
- cert_expires: Mar 14 20:59:59 2027 GMT
  host: mail.yandex.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yandex Mail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yandex Mail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yandex Mail
provider_slug: yandex-mail
slug: yandex-mail-domain-security
source_filename: yandex-mail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mail.yandex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 20:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: yandex.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/yandex-mail/security/yandex-mail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Communication
- Cloud
- Productivity
- Russian
---

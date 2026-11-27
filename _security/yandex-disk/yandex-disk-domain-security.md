---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yandex.com
  spf: true
hosts:
- cert_expires: Mar  1 20:59:59 2027 GMT
  host: disk.yandex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yandex Disk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yandex Disk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yandex Disk
provider_slug: yandex-disk
slug: yandex-disk-domain-security
source_filename: yandex-disk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: disk.yandex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 20:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yandex.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/yandex-disk/security/yandex-disk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Storage
- File Sync
- Backup
- AI Features
- Yandex 360
---

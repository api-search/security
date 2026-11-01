---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: translated.net
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: mymemory.translated.net
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mymemory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyMemory (Translated), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MyMemory (Translated)
provider_slug: mymemory
slug: mymemory-domain-security
source_filename: mymemory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mymemory.translated.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: translated.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mymemory/security/mymemory-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Translation
- API
- Localization
- Machine-Translation
---

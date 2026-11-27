---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infokmv.ru
  spf: true
hosts:
- cert_expires: Dec 21 17:12:25 2026 GMT
  host: infokmv.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: КМВ INFO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for КМВ INFO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: КМВ INFO
provider_slug: infokmv-ru
slug: infokmv-ru-domain-security
source_filename: infokmv-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infokmv.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 17:12:25 2026 GMT\n  hsts: false\ndomains:\n- domain: infokmv.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/infokmv-ru/security/infokmv-ru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Regional
- Russia
- Transportation
- Community
---

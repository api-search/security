---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: normaldance.ru
  spf: true
hosts:
- cert_expires: Dec 31 12:34:48 2026 GMT
  host: normaldance.ru
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: normaldance-ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for normaldance-ru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: normaldance-ru
provider_slug: normaldance-ru
slug: normaldance-ru-domain-security
source_filename: normaldance-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: normaldance.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 12:34:48 2026 GMT\n  hsts: null\ndomains:\n- domain: normaldance.ru\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/normaldance-ru/security/normaldance-ru-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: livsmedelsverket.se
  spf: true
hosts:
- cert_expires: Dec 21 03:41:48 2026 GMT
  host: www.livsmedelsverket.se
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Livsmedelsverket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Livsmedelsverket (Swedish Food Agency), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Livsmedelsverket (Swedish Food Agency)
provider_slug: livsmedelsverket
slug: livsmedelsverket-domain-security
source_filename: livsmedelsverket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.livsmedelsverket.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 03:41:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: livsmedelsverket.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/livsmedelsverket/security/livsmedelsverket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Food Safety
- Nutrition
- Sweden
---

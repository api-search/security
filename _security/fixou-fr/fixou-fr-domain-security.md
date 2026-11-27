---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fixou.fr
  spf: true
hosts:
- cert_expires: Dec 13 12:46:09 2026 GMT
  host: fixou.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fixou Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixou, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fixou
provider_slug: fixou-fr
slug: fixou-fr-domain-security
source_filename: fixou-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixou.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 12:46:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fixou.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fixou-fr/security/fixou-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Home Improvement
- Marketplace
- Artisan
- Service Platform
- France
---

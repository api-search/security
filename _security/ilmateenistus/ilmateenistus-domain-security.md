---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ilmateenistus.ee
  spf: true
hosts:
- cert_expires: Dec 31 17:30:18 2026 GMT
  host: ilmateenistus.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ilmateenistus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ilmateenistus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ilmateenistus
provider_slug: ilmateenistus
slug: ilmateenistus-domain-security
source_filename: ilmateenistus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ilmateenistus.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 17:30:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ilmateenistus.ee\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ilmateenistus/security/ilmateenistus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Weather
- Environment
- Estonia
- Government
- API
---

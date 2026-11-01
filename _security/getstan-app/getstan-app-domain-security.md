---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: getstan.app
  spf: true
hosts:
- cert_expires: Dec 21 20:40:06 2026 GMT
  host: getstan.app
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getstan App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Stan
provider_slug: getstan-app
slug: getstan-app-domain-security
source_filename: getstan-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getstan.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 20:40:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: getstan.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getstan-app/security/getstan-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Gaming
- Social
- CreatorEconomy
- Web3
---

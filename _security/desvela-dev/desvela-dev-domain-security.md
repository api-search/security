---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: desvela.dev
  spf: false
hosts:
- cert_expires: Dec  3 19:13:01 2026 GMT
  host: desvela.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Desvela Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for desvela-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: desvela-dev
provider_slug: desvela-dev
slug: desvela-dev-domain-security
source_filename: desvela-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: desvela.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 19:13:01 2026 GMT\n  hsts: false\ndomains:\n- domain: desvela.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/desvela-dev/security/desvela-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- BrandMonitoring
- Analytics
- SaaS
- Desvela
---

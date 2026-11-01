---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dowsure.com
  spf: true
hosts:
- cert_expires: Dec 17 02:52:23 2026 GMT
  host: world.dowsure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dowsure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dowsure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dowsure
provider_slug: dowsure
slug: dowsure-domain-security
source_filename: dowsure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: world.dowsure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 02:52:23 2026 GMT\n  hsts: false\ndomains:\n- domain: dowsure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dowsure/security/dowsure-domain-security.yml
summary_line: TLSv1.3
tags:
- Cross‑border E‑commerce Financing
- Embedded Finance
- API Banking
---

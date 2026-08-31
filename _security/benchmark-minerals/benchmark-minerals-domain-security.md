---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: benchmarkminerals.com
  spf: true
hosts:
- cert_expires: Aug 29 17:29:32 2026 GMT
  host: www.benchmarkminerals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 21:32:30 2026 GMT
  host: source.benchmarkminerals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Benchmark Minerals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benchmark Minerals, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Benchmark Minerals
provider_slug: benchmark-minerals
slug: benchmark-minerals-domain-security
source_filename: benchmark-minerals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benchmarkminerals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:29:32 2026 GMT\n  hsts: false\n- host: source.benchmarkminerals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:32:30 2026 GMT\n  hsts: false\ndomains:\n- domain: benchmarkminerals.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchmark-minerals/refs/heads/main/security/benchmark-minerals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Batteries
- Cobalt
- Critical Minerals
- Electric Vehicles
- Energy Transition
- Graphite
- Lithium
- Lithium Ion
- Market Intelligence
- Mining
- Nickel
- Price Reporting
- Rare Earths
- Supply Chain
---

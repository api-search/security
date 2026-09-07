---
api_specs:
- filename: benchmark-minerals-prices-api.yml
  format: yaml
  label: Benchmark Minerals API
  slug: benchmark-minerals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchmark-minerals/refs/heads/main/openapi/benchmark-minerals-prices-api.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: benchmarkminerals.com
  spf: true
hosts:
- cert_expires: Oct 27 23:23:43 2026 GMT
  host: www.benchmarkminerals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 06:14:39 2026 GMT
  host: source.benchmarkminerals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
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
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benchmarkminerals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:23:43 2026 GMT\n  hsts: false\n- host: source.benchmarkminerals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 06:14:39 2026 GMT\n  hsts: false\ndomains:\n- domain: benchmarkminerals.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
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
- Lithium-Ion
- Market Intelligence
- Mining
- Nickel
- Price Reporting
- Rare Earths
- Supply Chain
---

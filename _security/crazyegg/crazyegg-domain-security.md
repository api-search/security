---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crazyegg.com
  spf: true
hosts:
- cert_expires: Jan 18 23:47:39 2027 GMT
  host: www.crazyegg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crazy Egg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crazy Egg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crazy Egg
provider_slug: crazyegg
slug: crazyegg-domain-security
source_filename: crazyegg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crazyegg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:47:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crazyegg.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/crazyegg/security/crazyegg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Heatmaps
- Session Recording
- A/B Testing
- Conversion Optimization
- GraphQL
- MCP
---

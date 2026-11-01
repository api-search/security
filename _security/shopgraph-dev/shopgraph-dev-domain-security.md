---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: shopgraph.dev
  spf: false
hosts:
- cert_expires: Dec 24 23:36:31 2026 GMT
  host: shopgraph.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shopgraph Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shopgraph-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: shopgraph-dev
provider_slug: shopgraph-dev
slug: shopgraph-dev-domain-security
source_filename: shopgraph-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shopgraph.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:36:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shopgraph.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/shopgraph-dev/security/shopgraph-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-commerce
- GraphQL
- API
- DeveloperTools
---

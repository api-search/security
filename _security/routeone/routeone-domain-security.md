---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: routeone.com
  spf: true
hosts:
- cert_expires: Jan 23 14:34:22 2027 GMT
  host: routeone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RouteOne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RouteOne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RouteOne
provider_slug: routeone
slug: routeone-domain-security
source_filename: routeone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: routeone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 14:34:22 2027 GMT\n  hsts: null\ndomains:\n- domain: routeone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/routeone/security/routeone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Automotive
- Finance
- Insurance
- Dealership
---

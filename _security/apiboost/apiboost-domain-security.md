---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apiboost.com
  spf: true
hosts:
- cert_expires: Jan  9 04:21:16 2027 GMT
  host: apiboost.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apiboost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apiboost Developer Portals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apiboost Developer Portals
provider_slug: apiboost
slug: apiboost-domain-security
source_filename: apiboost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiboost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 04:21:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: apiboost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/apiboost/security/apiboost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Portal
- Developer Tools
- Multi-Gateway
- API Management
---

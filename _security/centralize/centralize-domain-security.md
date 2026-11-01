---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usecentralize.com
  spf: true
hosts:
- cert_expires: Jan  5 03:14:19 2027 GMT
  host: www.usecentralize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centralize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centralize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Centralize
provider_slug: centralize
slug: centralize-domain-security
source_filename: centralize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usecentralize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 03:14:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usecentralize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/centralize/security/centralize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Account Mapping
- CRM Integration
- Enterprise Sales
---

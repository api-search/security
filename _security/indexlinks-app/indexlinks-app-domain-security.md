---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: indexlinks.app
  spf: false
hosts:
- cert_expires: Jan  3 07:45:08 2027 GMT
  host: indexlinks.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: indexlinks-app Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for indexlinks-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: indexlinks-app
provider_slug: indexlinks-app
slug: indexlinks-app-domain-security
source_filename: indexlinks-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indexlinks.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 07:45:08 2027 GMT\n  hsts: null\ndomains:\n- domain: indexlinks.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/indexlinks-app/security/indexlinks-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---

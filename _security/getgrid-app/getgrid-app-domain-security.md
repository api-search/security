---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getgrid.app
  spf: true
hosts:
- cert_expires: Jan  1 23:38:03 2027 GMT
  host: getgrid.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getgrid App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Grid
provider_slug: getgrid-app
slug: getgrid-app-domain-security
source_filename: getgrid-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getgrid.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:38:03 2027 GMT\n  hsts: false\ndomains:\n- domain: getgrid.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getgrid-app/security/getgrid-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cash Advance
- PayBoost
---

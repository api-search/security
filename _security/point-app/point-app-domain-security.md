---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pointapp.org
  spf: true
hosts:
- cert_expires: Jan 23 00:07:31 2027 GMT
  host: pointapp.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Point App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for POINT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: POINT
provider_slug: point-app
slug: point-app-domain-security
source_filename: point-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pointapp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 00:07:31 2027 GMT\n  hsts: false\ndomains:\n- domain: pointapp.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/point-app/security/point-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---

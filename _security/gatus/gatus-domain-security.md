---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gatus.io
  spf: true
hosts:
- cert_expires: Jan 20 14:51:28 2027 GMT
  host: gatus.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gatus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gatus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gatus
provider_slug: gatus
slug: gatus-domain-security
source_filename: gatus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gatus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 14:51:28 2027 GMT\n  hsts: null\ndomains:\n- domain: gatus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gatus/security/gatus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Monitoring
- OpenSource
- StatusPage
- Alerting
- DevOps
---

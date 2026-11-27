---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fluentive.app
  spf: true
hosts:
- cert_expires: Jan  2 03:34:23 2027 GMT
  host: fluentive.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fluentive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluentive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fluentive
provider_slug: fluentive-app
slug: fluentive-app-domain-security
source_filename: fluentive-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluentive.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 03:34:23 2027 GMT\n  hsts: false\ndomains:\n- domain: fluentive.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fluentive-app/security/fluentive-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- CRM
- Scheduling
- Team Collaboration
- Freelancers
---

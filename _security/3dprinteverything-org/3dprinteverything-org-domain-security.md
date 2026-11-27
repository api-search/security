---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 3dprinteverything.org
  spf: true
hosts:
- cert_expires: Jan  6 18:44:55 2027 GMT
  host: 3dprinteverything.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3D Print Everything Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3D Print Everything, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 3D Print Everything
provider_slug: 3dprinteverything-org
slug: 3dprinteverything-org-domain-security
source_filename: 3dprinteverything-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 3dprinteverything.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 18:44:55 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: 3dprinteverything.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/3dprinteverything-org/security/3dprinteverything-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3D Printing
- Manufacturing
- B2B Services
- Rapid Prototyping
- Dallas-Fort Worth
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gleanit.co
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: gleanit.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gleanit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gleanit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gleanit
provider_slug: gleanit-co
slug: gleanit-co-domain-security
source_filename: gleanit-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gleanit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gleanit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gleanit-co/security/gleanit-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketing
- Analytics
- Agency
- Advertising
- Software-as-a-Service
---

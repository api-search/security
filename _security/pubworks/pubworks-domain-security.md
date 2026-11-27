---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gworks.com
  spf: true
hosts:
- cert_expires: Jan 22 07:12:45 2027 GMT
  host: gworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PubWorks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PubWorks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PubWorks
provider_slug: pubworks
slug: pubworks-domain-security
source_filename: pubworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 07:12:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pubworks/security/pubworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Municipal
- Software-as-a-Service
- Cloud
- Government
---

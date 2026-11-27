---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: neptivum.com
  spf: true
hosts:
- cert_expires: Feb  4 17:09:18 2027 GMT
  host: neptivum.com
  hsts: true
  hsts_max_age: 3
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Neptivum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neptivum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Neptivum
provider_slug: neptivum-com
slug: neptivum-com-domain-security
source_filename: neptivum-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neptivum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 17:09:18 2027 GMT\n  hsts: true\n  hsts_max_age: 3\ndomains:\n- domain: neptivum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/neptivum-com/security/neptivum-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marine
- Logbook
- Offline
- Navigation
- Sailing
---

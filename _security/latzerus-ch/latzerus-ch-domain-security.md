---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: latzerus.ch
  spf: true
hosts:
- cert_expires: Feb 10 10:25:50 2027 GMT
  host: latzerus.ch
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Latzerus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latzerus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Latzerus
provider_slug: latzerus-ch
slug: latzerus-ch-domain-security
source_filename: latzerus-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latzerus.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 10:25:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: latzerus.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/latzerus-ch/security/latzerus-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Sales
- Artificial Intelligence
- Education
- Switzerland
- Free
- Knowledge
---

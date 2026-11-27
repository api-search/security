---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intentwake.com
  spf: true
hosts:
- cert_expires: Jan  7 13:01:55 2027 GMT
  host: intentwake.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: intentwake-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for intentwake-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: intentwake-com
provider_slug: intentwake-com
slug: intentwake-com-domain-security
source_filename: intentwake-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intentwake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 13:01:55 2027 GMT\n  hsts: null\ndomains:\n- domain: intentwake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/intentwake-com/security/intentwake-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---

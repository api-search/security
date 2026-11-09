---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: folgpris.no
  spf: true
hosts:
- cert_expires: Jan 27 03:57:23 2027 GMT
  host: folgpris.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Folgpris No Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Følgpris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Følgpris
provider_slug: folgpris-no
slug: folgpris-no-domain-security
source_filename: folgpris-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: folgpris.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 03:57:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: folgpris.no\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/folgpris-no/security/folgpris-no-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---

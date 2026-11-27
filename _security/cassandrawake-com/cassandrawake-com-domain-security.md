---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cassandrawake.com
  spf: false
hosts:
- cert_expires: Jan  4 20:35:27 2027 GMT
  host: cassandrawake.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: cassandrawake-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cassandrawake-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: cassandrawake-com
provider_slug: cassandrawake-com
slug: cassandrawake-com-domain-security
source_filename: cassandrawake-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cassandrawake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 20:35:27 2027 GMT\n  hsts: null\ndomains:\n- domain: cassandrawake.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cassandrawake-com/security/cassandrawake-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

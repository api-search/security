---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dyntechinc.com
  spf: true
hosts:
- cert_expires: Jan  8 09:50:22 2027 GMT
  host: dyntechinc.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dyntech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamic Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dynamic Technologies
provider_slug: dyntech
slug: dyntech-domain-security
source_filename: dyntech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dyntechinc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 09:50:22 2027 GMT\n  hsts: false\ndomains:\n- domain: dyntechinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dyntech/security/dyntech-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---

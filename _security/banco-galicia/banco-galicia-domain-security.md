---
description: ''
domains:
- caa:
  - 128 issue "amazonaws.com"
  - 128 iodef "mailto:soc@bancogalicia.com.ar"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: galicia.ar
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: www.galicia.ar
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Banco Galicia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banco Galicia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Banco Galicia
provider_slug: banco-galicia
slug: banco-galicia-domain-security
source_filename: banco-galicia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.galicia.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: galicia.ar\n  dnssec: false\n  caa:\n  - 128 issue \"amazonaws.com\"\n  - 128 iodef \"mailto:soc@bancogalicia.com.ar\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/banco-galicia/security/banco-galicia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Finance
- Argentina
- Consumer Banking
---

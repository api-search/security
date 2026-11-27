---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: axenomia.cl
  spf: false
hosts:
- cert_expires: Jan  6 18:55:44 2027 GMT
  host: axenomia.cl
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: axenomia-cl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for axenomia-cl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: axenomia-cl
provider_slug: axenomia-cl
slug: axenomia-cl-domain-security
source_filename: axenomia-cl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axenomia.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 18:55:44 2027 GMT\n  hsts: null\ndomains:\n- domain: axenomia.cl\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/axenomia-cl/security/axenomia-cl-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

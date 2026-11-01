---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: imagetyperz.com
  spf: false
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: imagetyperz.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Imagetyperz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImageTyperz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ImageTyperz
provider_slug: imagetyperz
slug: imagetyperz-domain-security
source_filename: imagetyperz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imagetyperz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: imagetyperz.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/imagetyperz/security/imagetyperz-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- captcha
- automation
- api
- service
- image-processing
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: hadl.app
  spf: true
hosts:
- cert_expires: Jan 18 07:07:09 2027 GMT
  host: hadl.app
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HADL Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HADL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: HADL
provider_slug: hadl-app
slug: hadl-app-domain-security
source_filename: hadl-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hadl.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 07:07:09 2027 GMT\n  hsts: false\ndomains:\n- domain: hadl.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hadl-app/security/hadl-app-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
---

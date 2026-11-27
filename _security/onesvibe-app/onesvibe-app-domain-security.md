---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: onesvibe.app
  spf: true
hosts:
- cert_expires: Jan 19 11:13:13 2027 GMT
  host: onesvibe.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: onesvibe-app Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for onesvibe-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: onesvibe-app
provider_slug: onesvibe-app
slug: onesvibe-app-domain-security
source_filename: onesvibe-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onesvibe.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 11:13:13 2027 GMT\n  hsts: false\ndomains:\n- domain: onesvibe.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/onesvibe-app/security/onesvibe-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

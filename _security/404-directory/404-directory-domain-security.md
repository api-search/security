---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: 404.directory
  spf: false
hosts:
- cert_expires: Jan 12 18:22:10 2027 GMT
  host: 404.directory
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 404 Directory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 404-directory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: 404-directory
provider_slug: 404-directory
slug: 404-directory-domain-security
source_filename: 404-directory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 404.directory\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 18:22:10 2027 GMT\n  hsts: null\ndomains:\n- domain: 404.directory\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/404-directory/security/404-directory-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
---

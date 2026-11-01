---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: domainium.io
  spf: true
hosts:
- cert_expires: Jan  7 05:27:41 2027 GMT
  host: domainium.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domainium Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for domainium-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: domainium-io
provider_slug: domainium-io
slug: domainium-io-domain-security
source_filename: domainium-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domainium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 05:27:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: domainium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/domainium-io/security/domainium-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Domain
- Branding
- Tools
- API
---

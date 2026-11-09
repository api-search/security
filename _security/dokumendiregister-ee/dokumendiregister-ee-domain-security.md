---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: dokumendiregister.ee
  spf: false
hosts:
- cert_expires: Dec 16 17:29:53 2026 GMT
  host: dokumendiregister.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dokumendiregister Ee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dokumendi Register, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Dokumendi Register
provider_slug: dokumendiregister-ee
slug: dokumendiregister-ee-domain-security
source_filename: dokumendiregister-ee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dokumendiregister.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 17:29:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dokumendiregister.ee\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dokumendiregister-ee/security/dokumendiregister-ee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Government
- Estonia
- Public Data
- Search
- Free
---

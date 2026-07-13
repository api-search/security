---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: extendsclass.com
  spf: true
hosts:
- cert_expires: Sep 20 07:57:59 2026 GMT
  host: extendsclass.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Extendsclass Json Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExtendsClass JSON Storage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ExtendsClass JSON Storage
provider_slug: extendsclass-json-storage
slug: extendsclass-json-storage-domain-security
source_filename: extendsclass-json-storage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extendsclass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 07:57:59 2026 GMT\n  hsts: false\ndomains:\n- domain: extendsclass.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extendsclass-json-storage/refs/heads/main/security/extendsclass-json-storage-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Development
- Public APIs
---

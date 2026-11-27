---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dockai.co
  spf: false
hosts:
- cert_expires: Dec  6 18:29:08 2026 GMT
  host: dockai.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: dockai-co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dockai-co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: dockai-co
provider_slug: dockai-co
slug: dockai-co-domain-security
source_filename: dockai-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dockai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 18:29:08 2026 GMT\n  hsts: false\ndomains:\n- domain: dockai.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dockai-co/security/dockai-co-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

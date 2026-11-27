---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: idun.blue
  spf: true
hosts:
- cert_expires: Jan 17 15:18:44 2027 GMT
  host: idun.blue
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: idun-blue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for idun-blue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: idun-blue
provider_slug: idun-blue
slug: idun-blue-domain-security
source_filename: idun-blue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: idun.blue\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 15:18:44 2027 GMT\n  hsts: false\ndomains:\n- domain: idun.blue\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/idun-blue/security/idun-blue-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---

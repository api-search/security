---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bhasini.com
  spf: false
hosts:
- cert_expires: Jan 17 00:38:49 2027 GMT
  host: bhasini.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bhasini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bhasini, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Bhasini
provider_slug: bhasini-com
slug: bhasini-com-domain-security
source_filename: bhasini-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bhasini.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 00:38:49 2027 GMT\n  hsts: false\ndomains:\n- domain: bhasini.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bhasini-com/security/bhasini-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Typing
- Indian Languages
- Free
- Web App
- Utility
---

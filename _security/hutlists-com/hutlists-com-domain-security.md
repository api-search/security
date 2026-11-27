---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hutlists.com
  spf: true
hosts:
- cert_expires: Feb  8 17:07:54 2027 GMT
  host: hutlists.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HutLists Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HutLists, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HutLists
provider_slug: hutlists-com
slug: hutlists-com-domain-security
source_filename: hutlists-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hutlists.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 17:07:54 2027 GMT\n  hsts: false\ndomains:\n- domain: hutlists.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hutlists-com/security/hutlists-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Alpine
- Hiking
- MountainHuts
- Travel
- DataDirectory
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: konnectzit.com
  spf: true
hosts:
- cert_expires: Dec 17 03:12:25 2026 GMT
  host: konnectzit.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Konnectzit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KonnectzIT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KonnectzIT
provider_slug: konnectzit
slug: konnectzit-domain-security
source_filename: konnectzit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konnectzit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 03:12:25 2026 GMT\n  hsts: false\ndomains:\n- domain: konnectzit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/konnectzit/security/konnectzit-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
---

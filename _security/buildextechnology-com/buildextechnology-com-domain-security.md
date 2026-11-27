---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buildextechnology.com
  spf: true
hosts:
- cert_expires: Dec 20 13:25:03 2026 GMT
  host: buildextechnology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BUILDEX Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BUILDEX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BUILDEX
provider_slug: buildextechnology-com
slug: buildextechnology-com-domain-security
source_filename: buildextechnology-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildextechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 13:25:03 2026 GMT\n  hsts: false\ndomains:\n- domain: buildextechnology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buildextechnology-com/security/buildextechnology-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Modular Buildings
- Aluminium Ceilings
- Container Houses
- Prefabricated
- China
---

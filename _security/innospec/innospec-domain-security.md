---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: innospec.com
  spf: true
hosts:
- cert_expires: Sep 15 08:34:44 2026 GMT
  host: www.innospec.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.innospec.com
  https: false
- host: api.innospec.com
  https: false
kind: domain-security
layout: security
method: probed
name: Innospec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Innospec, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Innospec
provider_slug: innospec
slug: innospec-domain-security
source_filename: innospec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.innospec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:34:44 2026 GMT\n  hsts: false\n- host: developer.innospec.com\n  https: false\n- host: api.innospec.com\n  https: false\ndomains:\n- domain: innospec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innospec/refs/heads/main/security/innospec-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Specialty Chemicals
- Fuel Additives
---

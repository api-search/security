---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: akkilahdot.fi
  spf: true
hosts:
- cert_expires: Jan  3 04:27:44 2027 GMT
  host: akkilahdot.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Äkkilähdöt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Äkkilähdöt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Äkkilähdöt
provider_slug: akkilahdot-fi
slug: akkilahdot-fi-domain-security
source_filename: akkilahdot-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akkilahdot.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 04:27:44 2027 GMT\n  hsts: false\ndomains:\n- domain: akkilahdot.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/akkilahdot-fi/security/akkilahdot-fi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Finland
- Holiday
- Search
- Package
---

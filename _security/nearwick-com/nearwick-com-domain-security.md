---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nearwick.com
  spf: true
hosts:
- cert_expires: Dec 24 05:37:07 2026 GMT
  host: nearwick.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nearwick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nearwick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nearwick
provider_slug: nearwick-com
slug: nearwick-com-domain-security
source_filename: nearwick-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nearwick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 05:37:07 2026 GMT\n  hsts: false\ndomains:\n- domain: nearwick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nearwick-com/security/nearwick-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Directory
- Global
- Data
- Open Data
---

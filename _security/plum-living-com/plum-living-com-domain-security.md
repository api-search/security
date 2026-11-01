---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plum-living.com
  spf: true
hosts:
- cert_expires: Dec  2 21:30:16 2026 GMT
  host: www.plum-living.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Plum Living Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Plum
provider_slug: plum-living-com
slug: plum-living-com-domain-security
source_filename: plum-living-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plum-living.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 21:30:16 2026 GMT\n  hsts: null\ndomains:\n- domain: plum-living.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/plum-living-com/security/plum-living-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---

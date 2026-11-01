---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: withpulley.com
  spf: true
hosts:
- cert_expires: Dec  9 20:56:01 2026 GMT
  host: www.withpulley.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Withpulley Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulley, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pulley
provider_slug: withpulley-com
slug: withpulley-com-domain-security
source_filename: withpulley-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withpulley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 20:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: withpulley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/withpulley-com/security/withpulley-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---

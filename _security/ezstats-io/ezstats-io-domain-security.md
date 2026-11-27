---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ezstats.io
  spf: true
hosts:
- cert_expires: Feb  2 11:03:18 2027 GMT
  host: ezstats.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ezStats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ezStats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: ezStats
provider_slug: ezstats-io
slug: ezstats-io-domain-security
source_filename: ezstats-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ezstats.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 11:03:18 2027 GMT\n  hsts: false\ndomains:\n- domain: ezstats.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ezstats-io/security/ezstats-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Analytics
- SEO
- Artificial Intelligence
- Traffic
- Heatmaps
---

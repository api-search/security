---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fortellis.io
  spf: true
hosts:
- cert_expires: Dec 24 13:07:18 2026 GMT
  host: fortellis.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fortellis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortellis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fortellis
provider_slug: fortellis-io
slug: fortellis-io-domain-security
source_filename: fortellis-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fortellis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 13:07:18 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: fortellis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fortellis-io/security/fortellis-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Marketplace
- Developer Tools
- Platform
---

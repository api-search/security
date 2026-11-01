---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amo.co
  spf: true
hosts:
- cert_expires: Jan  1 12:06:58 2027 GMT
  host: www.amo.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amo
provider_slug: amo
slug: amo-domain-security
source_filename: amo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 12:06:58 2027 GMT\n  hsts: false\ndomains:\n- domain: amo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/amo/security/amo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Social
- Networking
- Apps
- Friendship
---

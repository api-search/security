---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ct-group.com
  spf: true
hosts:
- cert_expires: Nov 20 10:43:14 2026 GMT
  host: ct-group.com
  hsts: true
  hsts_max_age: 7884000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bigpicture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigpicture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bigpicture
provider_slug: bigpicture
slug: bigpicture-domain-security
source_filename: bigpicture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ct-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 10:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 7884000\ndomains:\n- domain: ct-group.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigpicture/refs/heads/main/security/bigpicture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Technology
- Services
- Events
- Creative
- Engineering
---

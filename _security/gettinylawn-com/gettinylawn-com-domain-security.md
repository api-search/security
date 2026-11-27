---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gettinylawn.com
  spf: true
hosts:
- cert_expires: Dec 28 14:47:24 2026 GMT
  host: gettinylawn.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tinylawn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tinylawn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tinylawn
provider_slug: gettinylawn-com
slug: gettinylawn-com-domain-security
source_filename: gettinylawn-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gettinylawn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 14:47:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gettinylawn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gettinylawn-com/security/gettinylawn-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Receptionist
- Landscaping
- Pest Control
- Software-as-a-Service
---

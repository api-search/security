---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dudko.dev
  spf: true
hosts:
- cert_expires: Dec 16 01:19:08 2026 GMT
  host: dudko.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dudko Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dudko-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: dudko-dev
provider_slug: dudko-dev
slug: dudko-dev-domain-security
source_filename: dudko-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dudko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 01:19:08 2026 GMT\n  hsts: false\ndomains:\n- domain: dudko.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dudko-dev/security/dudko-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software
- Consulting
- AI
- Open-Source
---

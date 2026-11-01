---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: palettelabs.com
  spf: true
hosts:
- cert_expires: Dec 28 22:16:37 2026 GMT
  host: palettelabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Palettelabs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palette 2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Palette 2
provider_slug: palettelabs-com
slug: palettelabs-com-domain-security
source_filename: palettelabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: palettelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 22:16:37 2026 GMT\n  hsts: false\ndomains:\n- domain: palettelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/palettelabs-com/security/palettelabs-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Media
- ContentCreation
- Platform
---

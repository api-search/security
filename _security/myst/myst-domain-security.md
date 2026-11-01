---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: myst.ai
  spf: true
hosts:
- cert_expires: Nov  3 03:08:51 2026 GMT
  host: www.myst.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Myst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Myst, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Myst
provider_slug: myst
slug: myst-domain-security
source_filename: myst-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myst.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 03:08:51 2026 GMT\n  hsts: false\ndomains:\n- domain: myst.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/myst/security/myst-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

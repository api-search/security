---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: jeikin.com
  spf: false
hosts:
- cert_expires: Dec 12 06:57:54 2026 GMT
  host: jeikin.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jeikin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jeikin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jeikin
provider_slug: jeikin-com
slug: jeikin-com-domain-security
source_filename: jeikin-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jeikin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 06:57:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jeikin.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jeikin-com/security/jeikin-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Accessibility
- Artificial Intelligence
- Compliance
- Developer Tools
---

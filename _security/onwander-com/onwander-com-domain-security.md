---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onwander.com
  spf: false
hosts:
- cert_expires: Dec 21 08:17:10 2026 GMT
  host: onwander.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Onwander Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wander *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Wander *
provider_slug: onwander-com
slug: onwander-com-domain-security
source_filename: onwander-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onwander.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 08:17:10 2026 GMT\n  hsts: false\ndomains:\n- domain: onwander.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/onwander-com/security/onwander-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Platform
- Startup
- Venture
- Technology
---

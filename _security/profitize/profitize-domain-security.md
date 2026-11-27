---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: profitize.com
  spf: false
hosts:
- cert_expires: Dec 22 05:16:28 2026 GMT
  host: profitize.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: profitize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for profitize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: profitize
provider_slug: profitize
slug: profitize-domain-security
source_filename: profitize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: profitize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 05:16:28 2026 GMT\n  hsts: null\ndomains:\n- domain: profitize.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/profitize/security/profitize-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
---

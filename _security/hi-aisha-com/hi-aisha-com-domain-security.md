---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hi-aisha.com
  spf: true
hosts:
- cert_expires: Dec 27 21:31:16 2026 GMT
  host: hi-aisha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hi Aisha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hi Aisha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hi Aisha
provider_slug: hi-aisha-com
slug: hi-aisha-com-domain-security
source_filename: hi-aisha-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hi-aisha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 21:31:16 2026 GMT\n  hsts: null\ndomains:\n- domain: hi-aisha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hi-aisha-com/security/hi-aisha-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---

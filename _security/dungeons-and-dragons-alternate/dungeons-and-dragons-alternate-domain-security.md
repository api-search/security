---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: open5e.com
  spf: false
hosts:
- cert_expires: Sep  4 10:05:19 2026 GMT
  host: open5e.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dungeons And Dragons Alternate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dungeons and Dragons (Alternate), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dungeons and Dragons (Alternate)
provider_slug: dungeons-and-dragons-alternate
slug: dungeons-and-dragons-alternate-domain-security
source_filename: dungeons-and-dragons-alternate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open5e.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 10:05:19 2026 GMT\n  hsts: false\ndomains:\n- domain: open5e.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dungeons-and-dragons-alternate/refs/heads/main/security/dungeons-and-dragons-alternate-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---

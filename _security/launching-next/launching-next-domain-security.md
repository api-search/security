---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: launchingnext.com
  spf: true
hosts:
- cert_expires: Sep  4 00:51:48 2026 GMT
  host: www.launchingnext.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Launching Next Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Launching Next, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Launching Next
provider_slug: launching-next
slug: launching-next-domain-security
source_filename: launching-next-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.launchingnext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 00:51:48 2026 GMT\n  hsts: false\ndomains:\n- domain: launchingnext.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launching-next/refs/heads/main/security/launching-next-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Discovery
- Product Launch
- Startups
---

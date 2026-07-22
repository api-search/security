---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: exide.com
  spf: false
hosts:
- cert_expires: Aug 26 18:03:12 2026 GMT
  host: www.exide.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exide Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exide Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Exide Technologies
provider_slug: exide-technologies
slug: exide-technologies-domain-security
source_filename: exide-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:03:12 2026 GMT\n  hsts: false\ndomains:\n- domain: exide.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exide-technologies/refs/heads/main/security/exide-technologies-domain-security.yml
summary_line: TLSv1.3
tags:
- Batteries
- Manufacturing
- Automotive
- Industrial
- Recycling
---

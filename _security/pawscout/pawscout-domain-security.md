---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pawscout.com
  spf: true
hosts:
- cert_expires: Dec  8 06:04:39 2026 GMT
  host: pawscout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pawscout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pawscout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pawscout
provider_slug: pawscout
slug: pawscout-domain-security
source_filename: pawscout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pawscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 06:04:39 2026 GMT\n  hsts: false\ndomains:\n- domain: pawscout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pawscout/refs/heads/main/security/pawscout-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Pet Safety
- Mobile App
- GPS Tags
- Community
---

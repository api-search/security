---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: telerik.com
  spf: true
hosts:
- cert_expires: Sep 16 21:12:01 2026 GMT
  host: www.telerik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fiddler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fiddler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fiddler
provider_slug: fiddler
slug: fiddler-domain-security
source_filename: fiddler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.telerik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 21:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: telerik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiddler/refs/heads/main/security/fiddler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Debugging
- HTTP Debugging
- HTTP Proxy
- Performance Testing
- Traffic Inspection
- Web Development
---

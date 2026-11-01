---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: modyfi.com
  spf: false
hosts:
- cert_expires: Jan 13 17:58:09 2027 GMT
  host: modyfi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Modyfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modyfi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Modyfi
provider_slug: modyfi
slug: modyfi-domain-security
source_filename: modyfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modyfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 17:58:09 2027 GMT\n  hsts: null\ndomains:\n- domain: modyfi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/modyfi/security/modyfi-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Startup
- VC-Backed
- API
- Stub
---

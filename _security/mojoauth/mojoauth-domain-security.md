---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: mojoauth.com
  spf: false
hosts:
- cert_expires: Oct  3 07:31:00 2026 GMT
  host: mojoauth.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mojoauth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MojoAuth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present.'
provider_name: MojoAuth
provider_slug: mojoauth
slug: mojoauth-domain-security
source_filename: mojoauth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mojoauth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:31:00 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: mojoauth.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mojoauth/refs/heads/main/security/mojoauth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication And Authorization
- Public APIs
---

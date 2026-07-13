---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: crafatar.com
  spf: false
hosts:
- cert_expires: Aug 31 05:29:33 2026 GMT
  host: crafatar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crafatar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crafatar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Crafatar
provider_slug: crafatar
slug: crafatar-domain-security
source_filename: crafatar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crafatar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:29:33 2026 GMT\n  hsts: null\ndomains:\n- domain: crafatar.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crafatar/refs/heads/main/security/crafatar-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Games And Comics
- Public APIs
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dicebear.com
  spf: true
hosts:
- cert_expires: Sep 17 11:01:50 2026 GMT
  host: avatars.dicebear.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dicebear Avatars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dicebear Avatars, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dicebear Avatars
provider_slug: dicebear-avatars
slug: dicebear-avatars-domain-security
source_filename: dicebear-avatars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avatars.dicebear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 11:01:50 2026 GMT\n  hsts: false\ndomains:\n- domain: dicebear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dicebear-avatars/refs/heads/main/security/dicebear-avatars-domain-security.yml
summary_line: TLSv1.3
tags:
- Test Data
- Public APIs
---

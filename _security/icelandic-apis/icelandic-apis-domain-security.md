---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apis.is
  spf: false
hosts:
- cert_expires: Aug 26 14:57:01 2026 GMT
  host: docs.apis.is
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Icelandic Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Icelandic APIs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Icelandic APIs
provider_slug: icelandic-apis
slug: icelandic-apis-domain-security
source_filename: icelandic-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.apis.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:57:01 2026 GMT\n  hsts: false\ndomains:\n- domain: apis.is\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icelandic-apis/refs/heads/main/security/icelandic-apis-domain-security.yml
summary_line: TLSv1.3
tags:
- Transportation
- Public APIs
---

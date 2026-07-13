---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openapihub.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: hub.openapihub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openapihub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAPIHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenAPIHub
provider_slug: openapihub
slug: openapihub-domain-security
source_filename: openapihub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hub.openapihub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: openapihub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openapihub/refs/heads/main/security/openapihub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Development
- Public APIs
---

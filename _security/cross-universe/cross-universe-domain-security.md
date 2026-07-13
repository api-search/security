---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: psychpsyo.com
  spf: true
hosts:
- cert_expires: Sep  8 09:51:41 2026 GMT
  host: crossuniverse.psychpsyo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cross Universe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cross Universe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cross Universe
provider_slug: cross-universe
slug: cross-universe-domain-security
source_filename: cross-universe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crossuniverse.psychpsyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:51:41 2026 GMT\n  hsts: null\ndomains:\n- domain: psychpsyo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cross-universe/refs/heads/main/security/cross-universe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games And Comics
- Public APIs
---

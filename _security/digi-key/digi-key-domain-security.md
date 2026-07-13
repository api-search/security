---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digikey.com
  spf: true
hosts:
- cert_expires: Aug 26 18:01:53 2026 GMT
  host: www.digikey.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digi Key Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digi-Key, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Digi-Key
provider_slug: digi-key
slug: digi-key-domain-security
source_filename: digi-key-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digikey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:01:53 2026 GMT\n  hsts: null\ndomains:\n- domain: digikey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/security/digi-key-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shopping
- Public APIs
---

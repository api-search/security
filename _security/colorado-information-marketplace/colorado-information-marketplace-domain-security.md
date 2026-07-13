---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: colorado.gov
  spf: true
hosts:
- cert_expires: Dec 17 12:50:44 2026 GMT
  host: data.colorado.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Colorado Information Marketplace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colorado Information Marketplace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Colorado Information Marketplace
provider_slug: colorado-information-marketplace
slug: colorado-information-marketplace-domain-security
source_filename: colorado-information-marketplace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.colorado.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 12:50:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: colorado.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colorado-information-marketplace/refs/heads/main/security/colorado-information-marketplace-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Government
- Public APIs
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hemnet.se
  spf: true
hosts:
- cert_expires: Dec  8 11:56:12 2026 GMT
  host: hemnet.se
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hemnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hemnet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hemnet
provider_slug: hemnet
slug: hemnet-domain-security
source_filename: hemnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hemnet.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 11:56:12 2026 GMT\n  hsts: null\ndomains:\n- domain: hemnet.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hemnet/refs/heads/main/security/hemnet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Marketplace
- Sweden
- Property Listings
---

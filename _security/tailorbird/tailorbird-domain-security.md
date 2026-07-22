---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tailorbird.com
  spf: true
hosts:
- cert_expires: Aug 22 08:43:33 2026 GMT
  host: www.tailorbird.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tailorbird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tailorbird, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tailorbird
provider_slug: tailorbird
slug: tailorbird-domain-security
source_filename: tailorbird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tailorbird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:43:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tailorbird.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailorbird/refs/heads/main/security/tailorbird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- PropTech
- Multifamily
- Construction
- Property Management
- CapEx
- Renovation
- Asset Management
- Artificial Intelligence
---

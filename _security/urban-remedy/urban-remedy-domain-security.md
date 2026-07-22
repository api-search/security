---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbanremedy.com
  spf: true
hosts:
- cert_expires: Oct 13 11:23:35 2026 GMT
  host: urbanremedy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urban Remedy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Remedy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Urban Remedy
provider_slug: urban-remedy
slug: urban-remedy-domain-security
source_filename: urban-remedy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanremedy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 11:23:35 2026 GMT\n  hsts: false\ndomains:\n- domain: urbanremedy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-remedy/refs/heads/main/security/urban-remedy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- Beverages
- Organic
- Wellness
- Cold-Pressed Juice
- Plant-Based
- Retail
---

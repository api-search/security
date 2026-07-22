---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pinhome.id
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: www.pinhome.id
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pinhome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinhome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pinhome
provider_slug: pinhome
slug: pinhome-domain-security
source_filename: pinhome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinhome.id\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pinhome.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinhome/refs/heads/main/security/pinhome-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Proptech
- Real Estate
- Property
- Mortgage
- Marketplace
- Indonesia
---

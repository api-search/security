---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_note: GoDaddy parking default DMARC record, not an operator-configured policy
  dmarc_policy: quarantine
  dmarc_rua: dmarc_rua@onsecureserver.net
  dnssec: false
  domain: landvault.io
  mx: false
  spf: false
hosts:
- cert_expires: Dec 10 14:03:36 2026 GMT
  cert_subject: CN=landvault.io
  host: landvault.io
  hsts: false
  https: true
  parked: true
  parking_provider: GoDaddy
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landvault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landvault, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Landvault
provider_slug: landvault
slug: landvault-domain-security
source_filename: landvault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the landvault.io domain of record\nnote: >-\n  landvault.io does not serve a company website. It resolves to GoDaddy parking\n  infrastructure (ns75/ns76.domaincontrol.com nameservers, a /lander redirect stub\n  served for every path, and parking-lander assets from img1.wsimg.com). The TLS\n  and DMARC values below therefore describe the registrar parking host, NOT\n  Landvault-operated infrastructure. Recorded as probe evidence that the domain is\n  no longer an active provider surface.\nhosts:\n- host: landvault.io\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=landvault.io\n  cert_expires: Dec 10 14:03:36 2026 GMT\n  hsts: false\n  parked: true\n  parking_provider: GoDaddy\ndomains:\n- domain: landvault.io\n  dnssec: false\n  caa: []\n  spf: false\n  mx: false\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: dmarc_rua@onsecureserver.net\n  dmarc_note: GoDaddy parking default\
  \ DMARC record, not an operator-configured policy\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landvault/refs/heads/main/security/landvault-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Portfolio Lead
- Speedinvest
- No API Surface
- Parked Domain
---

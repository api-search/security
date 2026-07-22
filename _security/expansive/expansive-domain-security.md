---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: expansive.mx
  spf: true
hosts:
- cert_expires: Oct 16 08:13:09 2026 GMT
  host: expansive.mx
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expansive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expansive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Expansive
provider_slug: expansive
slug: expansive-domain-security
source_filename: expansive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: expansive.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 08:13:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: expansive.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expansive/refs/heads/main/security/expansive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Real Estate
- Crowdfunding
- Investing
- Proptech
- Collective Financing
- Mexico
---

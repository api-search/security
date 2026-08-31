---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: waffleinsurance.com
  spf: true
hosts:
- cert_expires: Sep 11 18:41:13 2026 GMT
  host: www.waffleinsurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waffle Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waffle Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Waffle Labs
provider_slug: waffle-labs
slug: waffle-labs-domain-security
source_filename: waffle-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.waffleinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:41:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: waffleinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waffle-labs/refs/heads/main/security/waffle-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Fintech
- Consumer
- Embedded Insurance
- Renters Insurance
- Pet Insurance
- Techstars
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: assetreality.com
  spf: true
hosts:
- cert_expires: Sep 10 22:51:20 2026 GMT
  host: assetreality.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asset Reality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asset Reality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Asset Reality
provider_slug: asset-reality
slug: asset-reality-domain-security
source_filename: asset-reality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assetreality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:51:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: assetreality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asset-reality/refs/heads/main/security/asset-reality-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Asset Recovery
- Crypto Custody
- Digital Assets
- Law Enforcement
- GovTech
- RegTech
- Compliance
- Fraud
- Blockchain Forensics
---

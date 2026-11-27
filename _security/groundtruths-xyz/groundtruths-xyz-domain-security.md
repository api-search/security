---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: groundtruths.xyz
  spf: true
hosts:
- cert_expires: Jan 30 15:55:05 2027 GMT
  host: groundtruths.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GroundTruths Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GroundTruths, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GroundTruths
provider_slug: groundtruths-xyz
slug: groundtruths-xyz-domain-security
source_filename: groundtruths-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groundtruths.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 15:55:05 2027 GMT\n  hsts: false\ndomains:\n- domain: groundtruths.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/groundtruths-xyz/security/groundtruths-xyz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Prediction-Market
- Betting
- Analytics
- Finance
---

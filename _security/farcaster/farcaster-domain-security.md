---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: farcaster.xyz
  spf: true
hosts:
- cert_expires: Jul 23 00:13:16 2026 GMT
  host: www.farcaster.xyz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 03:07:29 2026 GMT
  host: snapchain.farcaster.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 14:18:34 2026 GMT
  host: miniapps.farcaster.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farcaster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farcaster, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Farcaster
provider_slug: farcaster
slug: farcaster-domain-security
source_filename: farcaster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.farcaster.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 23 00:13:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: snapchain.farcaster.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 03:07:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: miniapps.farcaster.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 14:18:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: farcaster.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farcaster/refs/heads/main/security/farcaster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Social
- Decentralized
- Protocol
- Mini Apps
- Frames
- Authentication
- Web3
- SDKs
---

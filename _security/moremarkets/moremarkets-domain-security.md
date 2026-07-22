---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moremarkets.xyz
  spf: true
hosts:
- cert_expires: Sep 17 00:12:30 2026 GMT
  host: www.moremarkets.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moremarkets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoreMarkets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MoreMarkets
provider_slug: moremarkets
slug: moremarkets-domain-security
source_filename: moremarkets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moremarkets.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 00:12:30 2026 GMT\n  hsts: null\ndomains:\n- domain: moremarkets.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moremarkets/refs/heads/main/security/moremarkets-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defi
- Yield
- Cross-Chain
- XRP
- Staking
- Vaults
- Crypto
---

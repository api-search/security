---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lifebeyondstudios.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: darewise.com
  note: web is offline but mail is still actively managed — Google Workspace MX, "v=spf1 include:_spf.google.com ~all", and DMARC p=quarantine pct=100 adkim=s aspf=s reporting to it-security@darewise.com.
  spf: true
hosts:
- cert_expires: Oct 18 16:38:30 2026 GMT
  host: www.lifebeyondstudios.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.darewise.com
  https: false
  note: legacy brand domain; DNS resolves to 139.177.176.71 but TCP 443 and 80 both refuse/time out, so no TLS or HSTS posture can be measured. Last Internet Archive capture serving HTTP 200 was 2025-04-21; captures from 2025-05-04 onward are 301s.
kind: domain-security
layout: security
method: probed
name: Darewise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Darewise, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Darewise
provider_slug: darewise
slug: darewise-domain-security
source_filename: darewise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lifebeyondstudios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 16:38:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.darewise.com\n  https: false\n  note: legacy brand domain; DNS resolves to 139.177.176.71 but TCP 443 and 80 both refuse/time out,\n    so no TLS or HSTS posture can be measured. Last Internet Archive capture serving HTTP 200 was\n    2025-04-21; captures from 2025-05-04 onward are 301s.\ndomains:\n- domain: lifebeyondstudios.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: darewise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  note: web is offline but mail is still actively managed — Google Workspace MX, \"v=spf1\n    include:_spf.google.com ~all\", and DMARC p=quarantine pct=100 adkim=s aspf=s reporting to\n    it-security@darewise.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/darewise/refs/heads/main/security/darewise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Games
- Game Development
- Web3
- NFT
- Metaverse
- Unreal Engine
- Entertainment
- Open-Source
---

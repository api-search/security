---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lindenlab.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: secondlife.com
  spf: true
hosts:
- cert_expires: Nov 19 19:44:48 2026 GMT
  host: lindenlab.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: wiki.secondlife.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.secondlife.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Linden Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linden Lab, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Linden Lab
provider_slug: linden-lab
slug: linden-lab-domain-security
source_filename: linden-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lindenlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 19:44:48 2026 GMT\n  hsts: false\n- host: wiki.secondlife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\n- host: api.secondlife.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lindenlab.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: secondlife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linden-lab/refs/heads/main/security/linden-lab-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Virtual Worlds
- Metaverse
- Gaming
- 3D
- Social
- Virtual Economy
- Digital Currency
- Marketplace
- Scripting
- User Generated Content
---

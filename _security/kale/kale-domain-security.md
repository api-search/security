---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getkale.com
  spf: true
hosts:
- cert_expires: Sep 14 15:02:01 2026 GMT
  host: www.getkale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kale
provider_slug: kale
slug: kale-domain-security
source_filename: kale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getkale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:02:01 2026 GMT\n  hsts: null\ndomains:\n- domain: getkale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kale/refs/heads/main/security/kale-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Creator Economy
- User-Generated Content
- Influencer Marketing
- Rewards
- Social Media
- Marketing
---

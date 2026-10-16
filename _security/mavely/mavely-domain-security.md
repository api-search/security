---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: joinmavely.com
  spf: true
hosts:
- cert_expires: Dec 10 23:51:51 2026 GMT
  host: www.joinmavely.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mavely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mavely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mavely
provider_slug: mavely
slug: mavely-domain-security
source_filename: mavely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinmavely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:51:51 2026 GMT\n  hsts: false\ndomains:\n- domain: joinmavely.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mavely/refs/heads/main/security/mavely-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Influencer
- CreatorPlatform
- AffiliateMarketing
- Monetization
---

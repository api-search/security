---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rayatheapp.com
  spf: true
hosts:
- cert_expires: Oct 16 00:19:51 2026 GMT
  host: www.rayatheapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Raya
provider_slug: raya
slug: raya-domain-security
source_filename: raya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rayatheapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:19:51 2026 GMT\n  hsts: false\ndomains:\n- domain: rayatheapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raya/refs/heads/main/security/raya-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Social Networking
- Dating
- Community
- Membership
- Mobile
- iOS
- Subscription
- Los Angeles
---

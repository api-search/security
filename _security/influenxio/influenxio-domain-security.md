---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: influenxio.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.influenxio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Influenxio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Influenxio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Influenxio
provider_slug: influenxio
slug: influenxio-domain-security
source_filename: influenxio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.influenxio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: influenxio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/influenxio/refs/heads/main/security/influenxio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Influencer Marketing
- Marketing
- Social Media
- Instagram
- Creator Economy
- Affiliate Marketing
- SaaS
---

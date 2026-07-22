---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zidisha.org
  spf: true
hosts:
- cert_expires: Aug 27 18:48:17 2026 GMT
  host: www.zidisha.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zidisha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zidisha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zidisha
provider_slug: zidisha
slug: zidisha-domain-security
source_filename: zidisha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zidisha.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:48:17 2026 GMT\n  hsts: false\ndomains:\n- domain: zidisha.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zidisha/refs/heads/main/security/zidisha-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Microlending
- Crowdfunding
- Fintech
- Nonprofit
- Financial Inclusion
- Philanthropy
- Peer to Peer Lending
---

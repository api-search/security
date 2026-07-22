---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_provider: Proofpoint Email Defense
  dnssec: false
  domain: masergy.com
  spf: true
  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all
hosts:
- cert_valid: true
  host: www.masergy.com
  hsts: false
  https: true
  redirects_to: https://business.comcast.com/masergy/
  tls_version: TLSv1.2
- host: api.masergy.com
  http_status: 502
  https: true
  live_api: false
  upstream: F5 Distributed Cloud (ves.io)
kind: domain-security
layout: security
method: probed
name: Masergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Masergy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Masergy
provider_slug: masergy
slug: masergy-domain-security
source_filename: masergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live TLS/HTTP HEAD + dig on masergy.com (2026-07-20)\nnote: >-\n  Masergy Communications was acquired by Comcast Business in October 2021 and\n  folded into Comcast Business. The masergy.com web hosts now 301-redirect to\n  business.comcast.com/masergy/. The domain's DNS + email records remain active\n  (Proofpoint-managed). No standalone Masergy API/developer surface is live:\n  api.masergy.com resolves to F5 Distributed Cloud but returns HTTP 502, and\n  developer.masergy.com / docs.masergy.com do not resolve.\nhosts:\n  - host: www.masergy.com\n    https: true\n    tls_version: TLSv1.2\n    cert_valid: true\n    hsts: false\n    redirects_to: https://business.comcast.com/masergy/\n  - host: api.masergy.com\n    https: true\n    http_status: 502\n    live_api: false\n    upstream: F5 Distributed Cloud (ves.io)\ndomains:\n  - domain: masergy.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com\
  \ ~all\"\n    dmarc: true\n    dmarc_policy: reject\n    dmarc_provider: Proofpoint Email Defense\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/masergy/refs/heads/main/security/masergy-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Networking
- SD-WAN
- SASE
- Managed Security
- Unified Communications
- Cloud Networking
- Enterprise
---

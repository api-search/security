---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: harbinger-health.com
  spf: true
hosts:
- cert_expires: Sep 10 00:47:15 2026 GMT
  host: harbinger-health.com
  hsts: null
  hsts_max_age: null
  https: true
  note: 'Fronted by Cloudflare (server: cloudflare). No Strict-Transport-Security header was returned on any probed path, so HSTS is not asserted for this origin.'
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Harbinger Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harbinger Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Harbinger Health
provider_slug: harbinger-health
slug: harbinger-health-domain-security
source_filename: harbinger-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the Harbinger Health host on 2026-08-04\nscope: >-\n  Only hosts Harbinger Health actually controls are recorded. The upstream documentation hosts\n  referenced from apis.yml humanURL fields (developer.wordpress.org, modelcontextprotocol.io) are\n  third-party and are deliberately excluded so their posture is not attributed to this provider.\nhosts:\n  - host: harbinger-health.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 10 00:47:15 2026 GMT\n    hsts: null\n    hsts_max_age: null\n    note: >-\n      Fronted by Cloudflare (server: cloudflare). No Strict-Transport-Security header was returned\n      on any probed path, so HSTS is not asserted for this origin.\ndomains:\n  - domain: harbinger-health.com\n    dnssec: true\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: none\nsubdomains_probed:\n  note: >-\n    None of the conventional developer, documentation,\
  \ API, portal, status or trust subdomains\n    resolve for this domain.\n  nxdomain:\n    - developer.harbinger-health.com\n    - docs.harbinger-health.com\n    - api.harbinger-health.com\n    - portal.harbinger-health.com\n    - status.harbinger-health.com\n    - trust.harbinger-health.com\nfindings:\n  strengths:\n    - TLS 1.3 negotiated on the only production host.\n    - DNSSEC is signed on harbinger-health.com.\n    - Both SPF and DMARC records are published.\n  gaps:\n    - No HSTS header, so the origin does not pin browsers or agents to HTTPS.\n    - No CAA record, so any public CA may issue for the domain.\n    - 'DMARC policy is p=none: reporting only, nothing is quarantined or rejected.'\n    - No /.well-known/security.txt (RFC 9116) is served.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbinger-health/refs/heads/main/security/harbinger-health-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Health
- Healthcare
- Biotechnology
- Cancer Detection
- Diagnostics
- Genomics
- Artificial Intelligence
- Machine Learning
- Life Sciences
- Clinical Laboratory
- Precision Medicine
- United States
- Company
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 6kinc.com
  spf: true
hosts:
- cert_expires: Oct 20 12:23:34 2026 GMT
  host: www.6kinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 6K Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 6K, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 6K
provider_slug: 6k
slug: 6k-domain-security
source_filename: 6k-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.6kinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 12:23:34 2026 GMT\n  hsts: false\ndomains:\n- domain: 6kinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6k/refs/heads/main/security/6k-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advanced Materials
- Manufacturing
- Additive Manufacturing
- Metal Powders
- Battery Materials
- Plasma Technology
- Energy Storage
- Aerospace
- Semiconductors
- Defense
- Sustainability
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: takecareos.com
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: takecareos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Takecareos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TakeCareOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TakeCareOS
provider_slug: takecareos
slug: takecareos-domain-security
source_filename: takecareos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: takecareos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: takecareos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/takecareos/refs/heads/main/security/takecareos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Home Care
- Long-Term Care
- Disability Services
- Compliance
- Scheduling
- Artificial Intelligence
- NDIS
- SaaS
---

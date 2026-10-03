---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biomason.com
  spf: true
hosts:
- cert_expires: Nov 26 08:52:57 2026 GMT
  host: biomason.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biomason Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biomason, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biomason
provider_slug: biomason
slug: biomason-domain-security
source_filename: biomason-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biomason.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 08:52:57 2026 GMT\n  hsts: false\ndomains:\n- domain: biomason.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biomason/refs/heads/main/security/biomason-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biotechnology
- Sustainable Construction
- Concrete
- Bioengineering
- Company
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cellincells.com
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: en.cellincells.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellincells Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellincells, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cellincells
provider_slug: cellincells
slug: cellincells-domain-security
source_filename: cellincells-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.cellincells.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cellincells.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellincells/refs/heads/main/security/cellincells-domain-security.yml
summary_line: TLSv1.3
tags:
- Biotechnology
- Regenerative Medicine
- Cell Therapy
- Artificial Intelligence
- South Korea
---

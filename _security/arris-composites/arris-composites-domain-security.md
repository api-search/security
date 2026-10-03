---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arriscomposites.com
  spf: true
hosts:
- cert_expires: Nov 22 04:00:42 2026 GMT
  host: arriscomposites.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arris Composites Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arris Composites, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Arris Composites
provider_slug: arris-composites
slug: arris-composites-domain-security
source_filename: arris-composites-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arriscomposites.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 04:00:42 2026 GMT\n  hsts: false\ndomains:\n- domain: arriscomposites.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arris-composites/refs/heads/main/security/arris-composites-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Manufacturing
- Composites
- AdditiveMolding
- Advanced Materials
---

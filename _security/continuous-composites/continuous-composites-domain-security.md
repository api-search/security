---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: continuouscomposites.com
  spf: true
hosts:
- cert_expires: Nov 11 09:57:12 2026 GMT
  host: continuouscomposites.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Continuous Composites Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Continuous Composites, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Continuous Composites
provider_slug: continuous-composites
slug: continuous-composites-domain-security
source_filename: continuous-composites-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: continuouscomposites.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 09:57:12 2026 GMT\n  hsts: false\ndomains:\n- domain: continuouscomposites.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continuous-composites/refs/heads/main/security/continuous-composites-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Aerospace
- Defense
- 3D Printing
- Composite Materials
---

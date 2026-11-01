---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cytrellis.com
  spf: true
hosts:
- cert_expires: Nov 23 15:28:45 2026 GMT
  host: www.cytrellis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cytrellis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cytrellis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cytrellis
provider_slug: cytrellis
slug: cytrellis-domain-security
source_filename: cytrellis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cytrellis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 15:28:45 2026 GMT\n  hsts: false\ndomains:\n- domain: cytrellis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cytrellis/security/cytrellis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aesthetic Devices
- Medical Technology
- FDA Cleared
- Skin Treatment
- Micro-Coring
---

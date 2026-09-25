---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cruzfoam.com
  spf: true
hosts:
- cert_expires: Sep 20 16:34:45 2026 GMT
  host: cruzfoam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cruz Foam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cruz Foam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cruz Foam
provider_slug: cruz-foam
slug: cruz-foam-domain-security
source_filename: cruz-foam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cruzfoam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:34:45 2026 GMT\n  hsts: false\ndomains:\n- domain: cruzfoam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/security/cruz-foam-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Materials Science
- Sustainable Packaging
- Compostable Materials
- Biomaterials
- Circular Economy
- Manufacturing
- Consumer Packaged Goods
- Cold Chain
- Sustainability
---

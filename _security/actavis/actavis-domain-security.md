---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: actavis.co.id
  spf: true
hosts:
- cert_expires: Nov 24 23:28:15 2026 GMT
  host: www.actavis.co.id
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Actavis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actavis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Actavis
provider_slug: actavis
slug: actavis-domain-security
source_filename: actavis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.actavis.co.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:28:15 2026 GMT\n  hsts: false\ndomains:\n- domain: actavis.co.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actavis/refs/heads/main/security/actavis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Generic Drugs
- Healthcare
- Manufacturing
- Acquired
---

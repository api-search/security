---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plos.org
  spf: true
hosts:
- cert_expires: Oct  6 14:11:02 2026 GMT
  host: plos.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.plos.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PLOS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PLOS
provider_slug: plos
slug: plos-domain-security
source_filename: plos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:11:02 2026 GMT\n  hsts: false\n- host: api.plos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plos.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plos/refs/heads/main/security/plos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scientific Articles
- Research
- Search
- Solr
- Open Access
---

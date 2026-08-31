---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: multiverse.io
  spf: true
hosts:
- cert_expires: Sep 24 10:10:09 2026 GMT
  host: www.multiverse.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Multiverse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Multiverse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Multiverse
provider_slug: multiverse
slug: multiverse-domain-security
source_filename: multiverse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.multiverse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:10:09 2026 GMT\n  hsts: false\ndomains:\n- domain: multiverse.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/multiverse/refs/heads/main/security/multiverse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Edtech
- Education
- Apprenticeships
- Workforce Development
- Upskilling
- Artificial Intelligence
- Training
---

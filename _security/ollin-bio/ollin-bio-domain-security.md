---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ollin.bio
  spf: true
hosts:
- cert_expires: Oct  7 20:00:43 2026 GMT
  host: ollin.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ollin Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ollin Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ollin Bio
provider_slug: ollin-bio
slug: ollin-bio-domain-security
source_filename: ollin-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ollin.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:00:43 2026 GMT\n  hsts: false\ndomains:\n- domain: ollin.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ollin-bio/refs/heads/main/security/ollin-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- Life Sciences
- Drug Development
- Pharmaceuticals
- a16z Portfolio
---

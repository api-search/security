---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cambrianbio.com
  spf: true
hosts:
- cert_expires: Oct  2 05:02:09 2026 GMT
  host: www.cambrianbio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cambrian Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambrian Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cambrian Bio
provider_slug: cambrian-bio
slug: cambrian-bio-domain-security
source_filename: cambrian-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cambrianbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:02:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cambrianbio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambrian-bio/refs/heads/main/security/cambrian-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Development
- Longevity
- Healthcare
- Life Sciences
- Clinical Stage
- Aging
- Metabolic Disease
---

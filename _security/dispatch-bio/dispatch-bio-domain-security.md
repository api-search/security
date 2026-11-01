---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dispatchbio.com
  spf: true
hosts:
- cert_expires: Dec 12 13:03:45 2026 GMT
  host: dispatchbio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dispatch Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dispatch Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dispatch Bio
provider_slug: dispatch-bio
slug: dispatch-bio-domain-security
source_filename: dispatch-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dispatchbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 13:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dispatchbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dispatch-bio/security/dispatch-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Immunotherapy
- Cancer
- Platform
- Startups
---

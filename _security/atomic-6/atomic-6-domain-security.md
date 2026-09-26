---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atomic-6.com
  spf: true
hosts:
- cert_expires: Dec 14 06:17:19 2026 GMT
  host: atomic-6.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atomic 6 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomic-6, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atomic-6
provider_slug: atomic-6
slug: atomic-6-domain-security
source_filename: atomic-6-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomic-6.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 06:17:19 2026 GMT\n  hsts: false\ndomains:\n- domain: atomic-6.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomic-6/refs/heads/main/security/atomic-6-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Composite Materials
- Space Technology
- Defense
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evozyne.com
  spf: true
hosts:
- cert_expires: Sep 24 00:00:28 2026 GMT
  host: evozyne.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evozyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evozyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Evozyne
provider_slug: evozyne
slug: evozyne-domain-security
source_filename: evozyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evozyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:00:28 2026 GMT\n  hsts: false\ndomains:\n- domain: evozyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evozyne/refs/heads/main/security/evozyne-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Artificial Intelligence
- Protein Design
- Drug Discovery
- Therapeutics
- Immunology
- Machine-Learning
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: biofidelity.com
  spf: true
hosts:
- cert_expires: Nov 22 02:00:16 2026 GMT
  host: biofidelity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biofidelity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biofidelity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Biofidelity
provider_slug: biofidelity
slug: biofidelity-domain-security
source_filename: biofidelity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biofidelity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 02:00:16 2026 GMT\n  hsts: null\ndomains:\n- domain: biofidelity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biofidelity/refs/heads/main/security/biofidelity-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Genomics
- Diagnostics
- Healthcare
---

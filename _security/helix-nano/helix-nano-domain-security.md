---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: helixnano.com
  spf: false
hosts:
- cert_expires: Sep 10 15:19:49 2026 GMT
  host: www.helixnano.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helix Nano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helix Nano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Helix Nano
provider_slug: helix-nano
slug: helix-nano-domain-security
source_filename: helix-nano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helixnano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:19:49 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: helixnano.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helix-nano/refs/heads/main/security/helix-nano-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- mRNA
- Vaccines
- Therapeutics
- Life Sciences
- Drug Discovery
---

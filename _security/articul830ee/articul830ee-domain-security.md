---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: articul8.ai
  spf: true
hosts:
- cert_expires: Nov 22 17:45:07 2026 GMT
  host: www.articul8.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Articul830Ee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Articul830ee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Articul830ee
provider_slug: articul830ee
slug: articul830ee-domain-security
source_filename: articul830ee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.articul8.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 17:45:07 2026 GMT\n  hsts: false\ndomains:\n- domain: articul8.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/articul830ee/refs/heads/main/security/articul830ee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Enterprise
- Platform
- DomainSpecific
---

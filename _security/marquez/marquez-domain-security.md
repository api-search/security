---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: marquezproject.ai
  spf: false
hosts:
- cert_expires: Dec 28 12:41:21 2026 GMT
  host: marquezproject.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marquez Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marquez, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Marquez
provider_slug: marquez
slug: marquez-domain-security
source_filename: marquez-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marquezproject.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 12:41:21 2026 GMT\n  hsts: false\ndomains:\n- domain: marquezproject.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marquez/refs/heads/main/security/marquez-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Open Source
- DataLineage
- Metadata
- OpenLineage
---

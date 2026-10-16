---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amundsen.io
  spf: false
hosts:
- cert_expires: Dec 24 10:44:07 2026 GMT
  host: www.amundsen.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amundsen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amundsen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Amundsen
provider_slug: amundsen
slug: amundsen-domain-security
source_filename: amundsen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amundsen.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 10:44:07 2026 GMT\n  hsts: false\ndomains:\n- domain: amundsen.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amundsen/refs/heads/main/security/amundsen-domain-security.yml
summary_line: TLSv1.3
tags:
- Data Discovery
- Open Source
- Metadata
- Search
- Governance
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Feb  9 00:53:06 2027 GMT
  host: tidybytetools.tidybytetools.workers.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tidy Byte Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tidy Byte Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tidy Byte Tools
provider_slug: tidybytetools
slug: tidybytetools-domain-security
source_filename: tidybytetools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tidybytetools.tidybytetools.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 00:53:06 2027 GMT\n  hsts: null\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tidybytetools/security/tidybytetools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Transformation
- Utilities
- Free
- Edge Computing
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: permianres.com
  spf: true
hosts:
- cert_expires: Aug 19 22:27:13 2026 GMT
  host: permianres.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Permian Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Permian Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Permian Resources
provider_slug: permian-resources
slug: permian-resources-domain-security
source_filename: permian-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: permianres.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 22:27:13 2026 GMT\n  hsts: false\ndomains:\n- domain: permianres.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permian-resources/refs/heads/main/security/permian-resources-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Oil and Gas
- Exploration and Production
- Permian Basin
- Upstream
---

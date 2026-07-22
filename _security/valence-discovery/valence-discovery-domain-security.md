---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: valencediscovery.com
  spf: true
hosts:
- cert_expires: Oct  2 00:15:15 2026 GMT
  host: valencediscovery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valence Discovery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valence Discovery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Valence Discovery
provider_slug: valence-discovery
slug: valence-discovery-domain-security
source_filename: valence-discovery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valencediscovery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:15:15 2026 GMT\n  hsts: false\ndomains:\n- domain: valencediscovery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valence-discovery/refs/heads/main/security/valence-discovery-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Drug Discovery
- Machine Learning
- Cheminformatics
- Molecular Design
- Artificial Intelligence
- Life Sciences
- Open Source
- Python
---

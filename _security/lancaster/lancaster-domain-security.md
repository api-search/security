---
api_specs:
- filename: lancaster-eprints-oai.yaml
  format: yaml
  label: Lancaster EPrints OAI-PMH
  slug: eprints-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancaster/refs/heads/main/openapi/lancaster-eprints-oai.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lancaster.ac.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lancs.ac.uk
  spf: true
hosts:
- cert_expires: Sep  6 02:43:23 2026 GMT
  host: www.lancaster.ac.uk
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 04:51:02 2026 GMT
  host: eprints.lancs.ac.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: developers.exlibrisgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lancaster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lancaster University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lancaster University
provider_slug: lancaster
slug: lancaster-domain-security
source_filename: lancaster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lancaster.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 02:43:23 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: eprints.lancs.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:51:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.exlibrisgroup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lancaster.ac.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lancs.ac.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lancaster/refs/heads/main/security/lancaster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research
- Library
- Open Data
---

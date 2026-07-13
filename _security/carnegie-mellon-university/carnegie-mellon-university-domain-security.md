---
api_specs:
- filename: carnegie-mellon-university-kilthub-figshare.yaml
  format: yaml
  label: KiltHub Repository OAI-PMH (figshare)
  slug: kilthub-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-kilthub-figshare.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cmu.edu
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.cmu.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 25 23:59:59 2026 GMT
  host: api.delphi.cmu.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 10:53:32 2026 GMT
  host: guides.library.cmu.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carnegie Mellon University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carnegie Mellon University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Carnegie Mellon University
provider_slug: carnegie-mellon-university
slug: carnegie-mellon-university-domain-security
source_filename: carnegie-mellon-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cmu.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.delphi.cmu.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 23:59:59 2026 GMT\n  hsts: null\n- host: guides.library.cmu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:53:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cmu.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/security/carnegie-mellon-university-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- United States
- Research
- Epidemiology
- Open Data
- Library
- Institutional Repository
---

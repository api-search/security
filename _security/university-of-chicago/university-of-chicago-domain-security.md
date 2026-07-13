---
api_specs:
- filename: university-of-chicago-fence.yaml
  format: yaml
  label: Gen3 Data Commons APIs (CTDS)
  slug: gen3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-chicago/refs/heads/main/openapi/university-of-chicago-fence.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: uchicago.edu
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: example.domain
  spf: false
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.uchicago.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: iiif-manifest.lib.uchicago.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: example.domain
  https: false
kind: domain-security
layout: security
method: probed
name: University Of Chicago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Chicago, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Chicago
provider_slug: university-of-chicago
slug: university-of-chicago-domain-security
source_filename: university-of-chicago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uchicago.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: iiif-manifest.lib.uchicago.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\n- host: example.domain\n  https: false\ndomains:\n- domain: uchicago.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: example.domain\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-chicago/refs/heads/main/security/university-of-chicago-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Source
- IIIF
- Identity
- United States
---

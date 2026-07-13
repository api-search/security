---
api_specs:
- filename: university-of-cambridge-lookup.yaml
  format: yaml
  label: Lookup / Ibis Web Service API
  slug: lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/openapi/university-of-cambridge-lookup.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cam.ac.uk
  spf: true
hosts:
- cert_expires: Aug 26 08:04:12 2026 GMT
  host: www.cam.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.lookup.cam.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:28:33 2026 GMT
  host: docs.raven.cam.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Cambridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Cambridge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: University of Cambridge
provider_slug: university-of-cambridge
slug: university-of-cambridge-domain-security
source_filename: university-of-cambridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cam.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 08:04:12 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.lookup.cam.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: docs.raven.cam.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:28:33 2026 GMT\n  hsts: false\ndomains:\n- domain: cam.ac.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/security/university-of-cambridge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- United Kingdom
- Identity
- API Gateway
- Developer Portal
---

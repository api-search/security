---
api_specs:
- filename: dartmouth-open-data.yaml
  format: yaml
  label: Dartmouth Open Data (ArcGIS Hub)
  slug: open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dartmouth/refs/heads/main/openapi/dartmouth-open-data.yaml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "emsign.com"
  - 0 issuemail "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dartmouth.edu
  spf: true
hosts:
- cert_expires: Aug 12 16:28:05 2026 GMT
  host: home.dartmouth.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug  1 23:59:59 2026 GMT
  host: developer.dartmouth.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 29 10:24:19 2026 GMT
  host: rc.dartmouth.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dartmouth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dartmouth College, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dartmouth College
provider_slug: dartmouth
slug: dartmouth-domain-security
source_filename: dartmouth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: home.dartmouth.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 12 16:28:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.dartmouth.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  1 23:59:59 2026 GMT\n  hsts: null\n- host: rc.dartmouth.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:24:19 2026 GMT\n  hsts: false\ndomains:\n- domain: dartmouth.edu\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"emsign.com\"\n  - 0 issuemail \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dartmouth/refs/heads/main/security/dartmouth-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Artificial Intelligence
- United States
- Ivy League
---

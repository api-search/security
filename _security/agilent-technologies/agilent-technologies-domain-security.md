---
api_specs:
- filename: agilent-ilab-operations-api.yaml
  format: yaml
  label: Agilent iLab Operations API
  slug: agilent-ilab-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/openapi/agilent-ilab-operations-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: agilent.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ilabsolutions.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.agilent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: help.ilab.agilent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.ilabsolutions.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Agilent Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agilent-technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: agilent-technologies
provider_slug: agilent-technologies
slug: agilent-technologies-domain-security
source_filename: agilent-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agilent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\n- host: help.ilab.agilent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ilabsolutions.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agilent.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ilabsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/security/agilent-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fortune 500
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
---

---
api_specs:
- filename: openapi-productionserver
  format: yaml
  label: MATLAB Production Server RESTful API
  slug: matlab-production-server-restful-api
  spec_type: OpenAPI
  url: https://github.com/mathworks-ref-arch/openapi-productionserver
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mathworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thingspeak.com
  spf: false
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.mathworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 23:59:59 2026 GMT
  host: api.thingspeak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matlab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MATLAB, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MATLAB
provider_slug: matlab
slug: matlab-domain-security
source_filename: matlab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mathworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\n- host: api.thingspeak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mathworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thingspeak.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matlab/refs/heads/main/security/matlab-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Analysis
- Engineering
- Machine Learning
- Numerical Analysis
- Scientific Computing
---

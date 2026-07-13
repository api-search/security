---
api_specs:
- filename: intel-trust-authority-api-openapi.yml
  format: yaml
  label: Intel Trust Authority API
  slug: trust-authority-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intel/refs/heads/main/openapi/intel-trust-authority-api-openapi.yml
- filename: intel-oneapi-openapi.yml
  format: yaml
  label: Intel oneAPI
  slug: oneapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intel/refs/heads/main/openapi/intel-oneapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: intel.com
  spf: true
hosts:
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: docs.trustauthority.intel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: api.trustauthority.intel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:59:59 2026 GMT
  host: www.intel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for intel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: intel
provider_slug: intel
slug: intel-domain-security
source_filename: intel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.trustauthority.intel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.trustauthority.intel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: null\n- host: www.intel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: intel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intel/refs/heads/main/security/intel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
---

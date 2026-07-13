---
api_specs:
- filename: scout-rfp-events-openapi.yml
  format: yaml
  label: Workday Strategic Sourcing API
  slug: workday-strategic-sourcing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scout-rfp/refs/heads/main/openapi/scout-rfp-events-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: workdayspend.com
  spf: false
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: apidocs.workdayspend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: api.us.workdayspend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.sandbox.us.workdayspend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scout Rfp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scout RFP, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Scout RFP
provider_slug: scout-rfp
slug: scout-rfp-domain-security
source_filename: scout-rfp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidocs.workdayspend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.us.workdayspend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\n- host: api.sandbox.us.workdayspend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: workdayspend.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scout-rfp/refs/heads/main/security/scout-rfp-domain-security.yml
summary_line: TLSv1.3
tags:
- Procurement
- Sourcing
- RFP
- Supply Chain
- Workday
---

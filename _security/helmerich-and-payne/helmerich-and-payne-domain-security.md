---
api_specs:
- filename: helmerich-and-payne-survey-validation-controller-api-openapi.yml
  format: yaml
  label: Helmerich & Payne Survey Validation Controller API
  slug: helmerich-and-payne-survey-validation-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helmerich-and-payne/refs/heads/main/openapi/helmerich-and-payne-survey-validation-controller-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hpinc.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: magvar.com
  spf: true
hosts:
- cert_expires: Dec  3 16:17:10 2026 GMT
  host: www.hpinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: fac-api.magvar.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Helmerich And Payne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helmerich & Payne, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Helmerich & Payne
provider_slug: helmerich-and-payne
slug: helmerich-and-payne-domain-security
source_filename: helmerich-and-payne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hpinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:17:10 2026 GMT\n  hsts: false\n- host: fac-api.magvar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: hpinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: magvar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helmerich-and-payne/refs/heads/main/security/helmerich-and-payne-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Oil and Gas
- Drilling
- Energy
- Wellbore Placement
- Directional Drilling
- Survey Management
- Geomagnetics
- Rig Automation
- Industrial
---

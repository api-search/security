---
api_specs:
- filename: europe-pmc-europepmc-api-openapi.yml
  format: yaml
  label: Europe PMC Europepmc API
  slug: europe-pmc-europepmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/europe-pmc/refs/heads/main/openapi/europe-pmc-europepmc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: europepmc.org
  spf: true
hosts:
- cert_expires: Nov 18 12:39:20 2026 GMT
  host: europepmc.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Europe Pmc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Europe PMC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Europe PMC
provider_slug: europe-pmc
slug: europe-pmc-domain-security
source_filename: europe-pmc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: europepmc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 12:39:20 2026 GMT\n  hsts: null\ndomains:\n- domain: europepmc.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/europe-pmc/refs/heads/main/security/europe-pmc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

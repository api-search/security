---
api_specs:
- filename: university-of-calgary-srs-api.yaml
  format: yaml
  label: UCalgary Space Remote Sensing API
  slug: srs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-srs-api.yaml
- filename: university-of-calgary-aurorax-api.yaml
  format: yaml
  label: AuroraX API
  slug: aurorax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-aurorax-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ucalgary.ca
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: aurorax.space
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.ucalgary.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api.phys.ucalgary.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 10:28:19 2026 GMT
  host: docs.aurorax.space
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Calgary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Calgary, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Calgary
provider_slug: university-of-calgary
slug: university-of-calgary-domain-security
source_filename: university-of-calgary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucalgary.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.phys.ucalgary.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\n- host: docs.aurorax.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:28:19 2026 GMT\n  hsts: false\ndomains:\n- domain: ucalgary.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aurorax.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/security/university-of-calgary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Repository
- Space Physics
- Canada
---

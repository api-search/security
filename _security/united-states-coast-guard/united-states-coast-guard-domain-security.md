---
api_specs:
- filename: cgmix-maritime-information-exchange-openapi.yml
  format: yaml
  label: CGMIX Maritime Information Exchange API
  slug: cgmix-maritime-information-exchange
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-coast-guard/refs/heads/main/openapi/cgmix-maritime-information-exchange-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uscg.mil
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uscg.gov
  spf: true
hosts:
- cert_expires: Feb 23 17:48:58 2027 GMT
  host: cgmix.uscg.mil
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.navcen.uscg.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: United States Coast Guard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United States Coast Guard, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: United States Coast Guard
provider_slug: united-states-coast-guard
slug: united-states-coast-guard-domain-security
source_filename: united-states-coast-guard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cgmix.uscg.mil\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 17:48:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.navcen.uscg.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: uscg.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: uscg.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-coast-guard/refs/heads/main/security/united-states-coast-guard-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Maritime Safety
- Vessel Documentation
- Emergency Response
- Law Enforcement
---

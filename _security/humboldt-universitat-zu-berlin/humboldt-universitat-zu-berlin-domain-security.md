---
api_specs:
- filename: humboldt-universitat-zu-berlin-edoc-rest.yaml
  format: yaml
  label: edoc-Server DSpace REST API
  slug: edoc-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/openapi/humboldt-universitat-zu-berlin-edoc-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hu-berlin.de
  spf: true
hosts:
- cert_expires: Nov 25 14:57:07 2026 GMT
  host: www.hu-berlin.de
  hsts: true
  hsts_max_age: 63115200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 00:17:05 2026 GMT
  host: edoc-info.hu-berlin.de
  hsts: true
  hsts_max_age: 63115200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 13:26:47 2026 GMT
  host: edoc.hu-berlin.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humboldt Universitat Zu Berlin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humboldt-Universität zu Berlin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Humboldt-Universität zu Berlin
provider_slug: humboldt-universitat-zu-berlin
slug: humboldt-universitat-zu-berlin-domain-security
source_filename: humboldt-universitat-zu-berlin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hu-berlin.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 14:57:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63115200\n- host: edoc-info.hu-berlin.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 00:17:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63115200\n- host: edoc.hu-berlin.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 13:26:47 2026 GMT\n  hsts: false\ndomains:\n- domain: hu-berlin.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/security/humboldt-universitat-zu-berlin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Library
- Germany
---

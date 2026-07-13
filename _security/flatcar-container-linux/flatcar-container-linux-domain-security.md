---
api_specs:
- filename: nebraska-update-api-openapi.yml
  format: yaml
  label: Flatcar Nebraska Update API
  slug: nebraska-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flatcar-container-linux/refs/heads/main/openapi/nebraska-update-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flatcar.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: flatcar-linux.org
  spf: false
hosts:
- cert_expires: Aug 19 07:02:28 2026 GMT
  host: www.flatcar.org
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- host: nebraska.flatcar-linux.org
  https: false
kind: domain-security
layout: security
method: probed
name: Flatcar Container Linux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flatcar Container Linux, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Flatcar Container Linux
provider_slug: flatcar-container-linux
slug: flatcar-container-linux-domain-security
source_filename: flatcar-container-linux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flatcar.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: nebraska.flatcar-linux.org\n  https: false\ndomains:\n- domain: flatcar.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: flatcar-linux.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flatcar-container-linux/refs/heads/main/security/flatcar-container-linux-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Containers
- Immutable Infrastructure
- Incubating
- Linux
- Operating System
---

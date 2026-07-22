---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pactpharma.com
  spf: true
hosts:
- cert_expires: Sep 17 22:49:35 2026 GMT
  host: pactpharma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pact Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PACT Pharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PACT Pharma
provider_slug: pact-pharma
slug: pact-pharma-domain-security
source_filename: pact-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pactpharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:49:35 2026 GMT\n  hsts: null\ndomains:\n- domain: pactpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pact-pharma/refs/heads/main/security/pact-pharma-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Life Sciences
- Biotechnology
- Cell Therapy
- Immunotherapy
- Oncology
---

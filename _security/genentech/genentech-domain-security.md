---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gene.com
  spf: true
hosts:
- cert_expires: Sep 19 23:46:37 2026 GMT
  host: www.gene.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: fhir.developer.gene.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.gene.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Genentech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genentech, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Genentech
provider_slug: genentech
slug: genentech-domain-security
source_filename: genentech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:46:37 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: fhir.developer.gene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\n- host: developer.gene.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: gene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genentech/refs/heads/main/security/genentech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Healthcare
- Life Sciences
- FHIR
- Patient Support Services
- Drug Discovery
- Genomics
---

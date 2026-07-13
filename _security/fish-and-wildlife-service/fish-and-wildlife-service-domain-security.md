---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fws.gov
  spf: true
hosts:
- cert_expires: Sep 24 14:11:15 2026 GMT
  host: www.fws.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: ecos.fws.gov
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Nov  9 11:39:40 2026 GMT
  host: ipac.ecosphere.fws.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fish And Wildlife Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for U.S. Fish and Wildlife Service, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: U.S. Fish and Wildlife Service
provider_slug: fish-and-wildlife-service
slug: fish-and-wildlife-service-domain-security
source_filename: fish-and-wildlife-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fws.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:11:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ecos.fws.gov\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: ipac.ecosphere.fws.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 11:39:40 2026 GMT\n  hsts: false\ndomains:\n- domain: fws.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fish-and-wildlife-service/refs/heads/main/security/fish-and-wildlife-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Conservation
- Endangered Species
- Federal Government
- Fisheries
- Wildlife
---

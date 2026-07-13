---
api_specs:
- filename: federal-railroad-administration-openapi.yml
  format: yaml
  label: Federal Railroad Administration Public API
  slug: federal-railroad-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-railroad-administration/refs/heads/main/openapi/federal-railroad-administration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dot.gov
  spf: true
hosts:
- host: www.fra.dot.gov
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- host: safetydata.fra.dot.gov
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Federal Railroad Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Railroad Administration, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Railroad Administration
provider_slug: federal-railroad-administration
slug: federal-railroad-administration-domain-security
source_filename: federal-railroad-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fra.dot.gov\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: safetydata.fra.dot.gov\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: dot.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-railroad-administration/refs/heads/main/security/federal-railroad-administration-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Federal Government
- Railroads
- Safety
- Transportation
---

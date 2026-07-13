---
api_specs:
- filename: squid-cache-manager-openapi.yml
  format: yaml
  label: Squid Cache Manager API
  slug: squid-cache-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squid/refs/heads/main/openapi/squid-cache-manager-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: squid-cache.org
  spf: true
hosts:
- host: www.squid-cache.org
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Squid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Squid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Squid
provider_slug: squid
slug: squid-domain-security
source_filename: squid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.squid-cache.org\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: squid-cache.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squid/refs/heads/main/security/squid-domain-security.yml
summary_line: DMARC
tags:
- Caching Proxy
- Proxy
- HTTP Proxy
- Web Cache
- Access Control
- Content Filtering
---

---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: HAProxy Data Plane API
  slug: haproxy-data-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/haproxytech/dataplaneapi/master/swagger.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: haproxy.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haproxy.com
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: www.haproxy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.haproxy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Haproxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HAProxy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HAProxy
provider_slug: haproxy
slug: haproxy-domain-security
source_filename: haproxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.haproxy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: www.haproxy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: haproxy.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: haproxy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haproxy/refs/heads/main/security/haproxy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- High Availability
- Load Balancing
- Networking
- Reverse Proxy
---

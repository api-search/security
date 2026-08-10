---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: omnidian.com
  spf: true
hosts:
- cert_expires: Oct 16 14:59:38 2026 GMT
  host: www.omnidian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.service.omnidian.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Omnidian API gateway (CNAME api-gateway-kube.service.omnidian.com); returns HTTP 401 anonymously on every probed path including /.well-known/*
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: client-portal.service.omnidian.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Omnidian Client Portal single-page app; answers HTTP 200 with an HTML shell for every path, including /.well-known/* (catch-all, not a discovery surface)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omnidian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omnidian, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Omnidian
provider_slug: omnidian
slug: omnidian-domain-security
source_filename: omnidian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omnidian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:59:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.service.omnidian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: 'Omnidian API gateway (CNAME api-gateway-kube.service.omnidian.com); returns\n    HTTP 401 anonymously on every probed path including /.well-known/*'\n- host: client-portal.service.omnidian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: 'Omnidian Client Portal single-page app; answers HTTP 200 with an HTML shell\n    for every path, including /.well-known/* (catch-all, not a discovery surface)'\ndomains:\n- domain:\
  \ omnidian.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnidian/refs/heads/main/security/omnidian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Solar
- Clean Energy
- Renewable Energy
- Asset Management
- Monitoring
- Performance Assurance
- Battery Storage
- Field Service
---

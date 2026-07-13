---
api_specs:
- filename: packagist-api-openapi.yml
  format: yaml
  label: Packagist API
  slug: packagist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packagist/refs/heads/main/openapi/packagist-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 iodef "mailto:security@packagist.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: packagist.org
  spf: true
hosts:
- cert_expires: Oct  8 19:01:53 2026 GMT
  host: packagist.org
  hsts: true
  hsts_max_age: 31104000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 01:01:59 2026 GMT
  host: repo.packagist.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Packagist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packagist, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Packagist
provider_slug: packagist
slug: packagist-domain-security
source_filename: packagist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packagist.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:01:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31104000\n- host: repo.packagist.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:01:59 2026 GMT\n  hsts: null\ndomains:\n- domain: packagist.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:security@packagist.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packagist/refs/heads/main/security/packagist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Composer
- PHP
- Package Registry
- Dependency Management
- Open Source
- Developer Tools
- Software Supply Chain
- Security Advisories
---

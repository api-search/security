---
api_specs:
- filename: php-fpm-openapi.yml
  format: yaml
  label: PHP-FPM Status Endpoint
  slug: status-endpoint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/php-fpm/refs/heads/main/openapi/php-fpm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: php.net
  spf: true
hosts:
- cert_expires: Sep  8 09:13:57 2026 GMT
  host: www.php.net
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Php Fpm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PHP-FPM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PHP-FPM
provider_slug: php-fpm
slug: php-fpm-domain-security
source_filename: php-fpm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.php.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:13:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: php.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/php-fpm/refs/heads/main/security/php-fpm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PHP
- FastCGI
- Process Manager
- Web Server
- Application Server
- Open Source
---

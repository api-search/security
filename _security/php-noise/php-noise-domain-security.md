---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: php-noise.com
  spf: false
hosts:
- cert_expires: Sep 30 11:31:00 2026 GMT
  host: php-noise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Php Noise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PHP-Noise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PHP-Noise
provider_slug: php-noise
slug: php-noise-domain-security
source_filename: php-noise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: php-noise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:31:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: php-noise.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/php-noise/refs/heads/main/security/php-noise-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Art And Design
- Public APIs
---

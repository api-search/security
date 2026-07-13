---
api_specs:
- filename: wordpress-rest-api-openapi.yml
  format: yaml
  label: WordPress REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wp-cli.org
  spf: false
hosts:
- cert_expires: Aug 24 19:43:58 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 19:44:09 2026 GMT
  host: wp-cli.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wordpress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WordPress, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WordPress
provider_slug: wordpress
slug: wordpress-domain-security
source_filename: wordpress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:43:58 2026 GMT\n  hsts: false\n- host: wp-cli.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:44:09 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wp-cli.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/security/wordpress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- Open Source
- WordPress
---

---
api_specs:
- filename: abcuro-content-openapi.yml
  format: yaml
  label: Abcuro Content API (WordPress REST)
  slug: abcuro-content-api-wordpress-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abcuro.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 25 01:57:06 2026 GMT
  host: abcuro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abcuro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abcuro, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Abcuro
provider_slug: abcuro
slug: abcuro-domain-security
source_filename: abcuro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abcuro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 01:57:06 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: abcuro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/security/abcuro-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- biotechnology
- pharmaceuticals
- immunology
- autoimmune-disease
- oncology
- clinical-trials
- life-sciences
- drug-development
- healthcare
- content-api
- wordpress
---

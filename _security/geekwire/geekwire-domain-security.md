---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: GeekWire WordPress REST API
  slug: wordpress-rest-api
  spec_type: OpenAPI
  url: https://www.geekwire.com/wp-json/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: geekwire.com
  spf: true
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep  4 16:46:27 2026 GMT
  host: www.geekwire.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:43:58 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geekwire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeekWire, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: GeekWire
provider_slug: geekwire
slug: geekwire-domain-security
source_filename: geekwire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geekwire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 16:46:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:43:58 2026 GMT\n  hsts: false\ndomains:\n- domain: geekwire.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geekwire/refs/heads/main/security/geekwire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Media
- Startups
- Technology News
---

---
api_specs:
- filename: dnsimple-openapi.yml
  format: yaml
  label: DNSimple API
  slug: dnsimple
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:ops@dnsimple.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dnsimple.com
  spf: true
hosts:
- cert_expires: Oct  3 20:03:39 2026 GMT
  host: developer.dnsimple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 23:59:59 2026 GMT
  host: api.dnsimple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dnsimple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNSimple, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DNSimple
provider_slug: dnsimple
slug: dnsimple-domain-security
source_filename: dnsimple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.dnsimple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:03:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dnsimple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dnsimple.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:ops@dnsimple.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/security/dnsimple-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DNS
- Domains
---

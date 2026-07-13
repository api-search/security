---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@postman.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: httpbin.org
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: httpbin.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Httpbin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Httpbin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Httpbin
provider_slug: httpbin
slug: httpbin-domain-security
source_filename: httpbin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: httpbin.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: httpbin.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@postman.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/httpbin/refs/heads/main/security/httpbin-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Development
- Public APIs
---

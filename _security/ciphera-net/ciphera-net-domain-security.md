---
api_specs:
- filename: ciphera-net-openapi-generated.yml
  format: yaml
  label: Ciphera API
  slug: ciphera-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ciphera-net/openapi/_ae-authored/ciphera-net-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:postmaster@ciphera.net"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ciphera.net
  spf: true
hosts:
- cert_expires: Jan 22 18:01:50 2027 GMT
  host: ciphera.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ciphera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ciphera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ciphera
provider_slug: ciphera-net
slug: ciphera-net-domain-security
source_filename: ciphera-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ciphera.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 18:01:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ciphera.net\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:postmaster@ciphera.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ciphera-net/security/ciphera-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Privacy
- Security
- Europe
- Open Source
---

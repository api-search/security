---
api_specs:
- filename: dns-openapi.yml
  format: yaml
  label: Google Cloud DNS API
  slug: google-cloud-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dns/refs/heads/main/openapi/dns-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: dns.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Cloud Dns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud DNS, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud DNS
provider_slug: google-cloud-dns
slug: google-cloud-dns-domain-security
source_filename: google-cloud-dns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dns.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dns/refs/heads/main/security/google-cloud-dns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DNS
- Domain Names
- Google Cloud
- Name Resolution
- Networking
---

---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signifyapp.com
  spf: true
hosts:
- cert_expires: Apr 19 23:59:59 2027 GMT
  host: signifyapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Signifyapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Signify
provider_slug: signifyapp
slug: signifyapp-domain-security
source_filename: signifyapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signifyapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: signifyapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/signifyapp/security/signifyapp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Contract Management
- Digital Signature
- Enterprise Software
- Software-as-a-Service
---

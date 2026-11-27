---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: glitterball.dev
  spf: true
hosts:
- cert_expires: Jan 10 14:01:08 2027 GMT
  host: glitterball.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Glitterball Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glitterball, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Glitterball
provider_slug: glitterball-dev
slug: glitterball-dev-domain-security
source_filename: glitterball-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glitterball.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 14:01:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: glitterball.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/glitterball-dev/security/glitterball-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Interactive
- Prototypes
- Feedback
- Video
---

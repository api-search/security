---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: igods.com
  spf: true
hosts:
- cert_expires: Dec 18 12:11:57 2026 GMT
  host: igods.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Igods Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for igods-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: igods-com
provider_slug: igods-com
slug: igods-com-domain-security
source_filename: igods-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: igods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:11:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: igods.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/igods-com/security/igods-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Internet-Marketing
- SEO
- Analytics
- WordPress
- Consulting
---

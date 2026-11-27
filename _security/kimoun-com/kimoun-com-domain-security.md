---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:dns-master@kimoun.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kimoun.com
  spf: true
hosts:
- cert_expires: Feb  6 15:58:10 2027 GMT
  host: kimoun.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kimoun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kimoun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kimoun
provider_slug: kimoun-com
slug: kimoun-com-domain-security
source_filename: kimoun-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kimoun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 15:58:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kimoun.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:dns-master@kimoun.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kimoun-com/security/kimoun-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SEO
- Digital Services
---

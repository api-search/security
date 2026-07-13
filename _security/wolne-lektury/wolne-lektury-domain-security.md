---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wolnelektury.pl
  spf: true
hosts:
- cert_expires: Sep 15 03:05:59 2026 GMT
  host: wolnelektury.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wolne Lektury Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wolne Lektury, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Wolne Lektury
provider_slug: wolne-lektury
slug: wolne-lektury-domain-security
source_filename: wolne-lektury-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wolnelektury.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:05:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wolnelektury.pl\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolne-lektury/refs/heads/main/security/wolne-lektury-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Books
- Public APIs
---

---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:info@koofr.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: koofr.eu
  spf: true
hosts:
- cert_expires: Jan 24 10:08:32 2027 GMT
  host: koofr.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Koofr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koofr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Koofr
provider_slug: koofr
slug: koofr-domain-security
source_filename: koofr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koofr.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 10:08:32 2027 GMT\n  hsts: false\ndomains:\n- domain: koofr.eu\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:info@koofr.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/koofr/security/koofr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Storage
- Privacy
- GDPR
- File Sync
- European Union
- Company
---

---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:data@jellyfish.co"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jellyfish.co
  spf: true
hosts:
- cert_expires: Aug 23 08:11:36 2026 GMT
  host: jellyfish.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jellyfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jellyfish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jellyfish
provider_slug: jellyfish
slug: jellyfish-domain-security
source_filename: jellyfish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jellyfish.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jellyfish.co\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:data@jellyfish.co\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jellyfish/refs/heads/main/security/jellyfish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Engineering Intelligence
- Engineering Management
- Developer Productivity
- Software Development
- DevOps
- Analytics
---

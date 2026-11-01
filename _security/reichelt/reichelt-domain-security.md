---
description: ''
domains:
- caa:
  - 0 iodef "mailto:webmaster@reichelt.de"
  - 0 issue "Digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reichelt.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.reichelt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reichelt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reichelt Elektronik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reichelt Elektronik
provider_slug: reichelt
slug: reichelt-domain-security
source_filename: reichelt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reichelt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reichelt.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:webmaster@reichelt.de\"\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/reichelt/security/reichelt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electronics
- Retail
- Components
- Hobbyist
- Professional
---

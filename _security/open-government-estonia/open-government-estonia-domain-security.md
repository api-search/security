---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:report@ria.ee"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eesti.ee
  spf: true
hosts:
- cert_expires: Aug  3 21:05:45 2026 GMT
  host: avaandmed.eesti.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Estonia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Estonia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Open Government, Estonia
provider_slug: open-government-estonia
slug: open-government-estonia-domain-security
source_filename: open-government-estonia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avaandmed.eesti.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 21:05:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eesti.ee\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:report@ria.ee\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-estonia/refs/heads/main/security/open-government-estonia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Public APIs
---

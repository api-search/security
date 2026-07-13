---
description: ''
domains:
- caa:
  - 128 issuewild "letsencrypt.org"
  - 128 iodef "mailto:prodhosting@utah.gov"
  - 128 issue "letsencrypt.org"
  - 128 issue "sectigo.com"
  - 128 issue "amazon.com"
  - 128 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: utah.gov
  spf: true
hosts:
- cert_expires: Sep 28 03:35:31 2026 GMT
  host: api.mapserv.utah.gov
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Utah Agrc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Utah AGRC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Utah AGRC
provider_slug: utah-agrc
slug: utah-agrc-domain-security
source_filename: utah-agrc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.mapserv.utah.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 03:35:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: utah.gov\n  dnssec: true\n  caa:\n  - 128 issuewild \"letsencrypt.org\"\n  - 128 iodef \"mailto:prodhosting@utah.gov\"\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"amazon.com\"\n  - 128 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utah-agrc/refs/heads/main/security/utah-agrc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Geocoding
- Public APIs
---

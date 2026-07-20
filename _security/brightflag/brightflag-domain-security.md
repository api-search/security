---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:caareport@brightflag.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightflag.com
  spf: true
hosts:
- cert_expires: Sep 14 18:57:16 2026 GMT
  host: brightflag.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightflag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brightflag, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brightflag
provider_slug: brightflag
slug: brightflag-domain-security
source_filename: brightflag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brightflag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:57:16 2026 GMT\n  hsts: false\ndomains:\n- domain: brightflag.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:caareport@brightflag.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightflag/refs/heads/main/security/brightflag-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Legal
- Legal Operations
- Legal Spend Management
- Enterprise Legal Management
- E-Billing
- Matter Management
- Reporting
- Artificial Intelligence
- LegalTech
---

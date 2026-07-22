---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:systems@unmortgage.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wayhome.co.uk
  spf: true
hosts:
- cert_expires: Sep 18 00:03:57 2026 GMT
  host: wayhome.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wayhome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wayhome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wayhome
provider_slug: wayhome
slug: wayhome-domain-security
source_filename: wayhome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wayhome.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:03:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wayhome.co.uk\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:systems@unmortgage.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayhome/refs/heads/main/security/wayhome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proptech
- Fintech
- Real Estate
- Homeownership
- Mortgage Alternative
- Shared Ownership
- United Kingdom
---

---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomberg.com
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomberg Valuation Service Bval Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg Valuation Service (BVAL), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg Valuation Service (BVAL)
provider_slug: bloomberg-valuation-service-bval
slug: bloomberg-valuation-service-bval-domain-security
source_filename: bloomberg-valuation-service-bval-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bloomberg.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-valuation-service-bval/refs/heads/main/security/bloomberg-valuation-service-bval-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- BVAL
- Evaluated Pricing
- Fixed Income
- Fair Value
- Bond Pricing
- Municipal Bonds
- Structured Products
- Bloomberg
---

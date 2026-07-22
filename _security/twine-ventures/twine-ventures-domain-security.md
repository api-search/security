---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: twineventures.com
  spf: true
hosts:
- cert_expires: Oct  1 01:27:31 2026 GMT
  host: www.twineventures.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twine Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twine Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Twine Ventures
provider_slug: twine-ventures
slug: twine-ventures-domain-security
source_filename: twine-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twineventures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:27:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: twineventures.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twine-ventures/refs/heads/main/security/twine-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Venture Capital
- Venture Firm
- Investor
- Early Stage
- Healthcare
- Industrials
- Fintech
- Data
- AI
---
